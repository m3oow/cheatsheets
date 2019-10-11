# Cheatsheet for Linux enumeration

## Table of contents
* [Kernel, OS & devices](#_kernel)
* [Users & groups](#_users)
* [User & Privilege Information](#_privileges)
* [Environmental Information](#_env)
* [Interesting Files](#_files)

## Kernel, OS & devices <a name="_kernel"></a>
Command | Result
------------ | -------------
`uname -a` | Print all available system information
`uname -r` | Kernel release
`uname -n` | System hostname
`uname -m` | Linux kernel architecture (32 or 64 bit)
`hostname` | As above
`cat /proc/version` | Kernel information
`cat /etc/*-release` | Distribution information
`cat /etc/issue` | As above
`cat /proc/cpuinfo` | CPU information
`df -a` | File system information

## Users & Groups <a name="_users"></a>
Command | Result
------------ | -------------
`cat /etc/passwd` | List all users on the system
`cat /etc/group` | List all groups on the system
`for i in $(cat /etc/passwd 2> /dev/null \| cut -d ":" -f1 2> /dev/null); do id $i; done 2> /dev/null` | List all uid’s and respective group memberships
`cat /etc/shadow` | Show user hashes – Privileged command
`grep -v -E "^#" /etc/passwd \| awk -F: '$3 == 0 { print $1 }'` | List all super user accounts
`finger` | Users currently logged in
`pinky` | As above
`users` | As above
`who -a` | As above
`w` | Who is currently logged in and what they’re doing
`last` | Listing of last logged on users
`lastlog` | Information on when all users last logged in
`lastlog –u %username%` | Information on when the specified user last | logged in
`lastlog \| grep -v "Never"` | Entire list of previously logged on users

## User & Privilege Information <a name="_privileges"></a>
Command | Result
------------ | -------------
`whoami` | Current username
`id` | Current user information
`cat /etc/sudoers` | Who’s allowed to do what as root – Privileged command
`sudo -l` | Can the current user perform anything as root

## Environmental Information <a name="_env"></a>
Command | Result
------------ | -------------
`env` | Display environmental variables
`set` | As above
`echo $PATH` | Path information
`history` | Displays command history of current user
`pwd` | Print working directory, i.e. ‘where am I’
`cat /etc/profile` | Display default system variables
`cat /etc/shells` | Display available shells

## Interesting Files <a name="_files"></a>
Command | Result
------------ | -------------
`find / -perm -4000 -type f 2>/dev/null` | Find SUID files
`find / -uid 0 -perm -4000 -type f 2> /dev/null` | Find SUID files owned by root
`find / -perm -2000 -type f 2> /dev/null` | Find GUID files
`find / -perm -2 -type f 2> /dev/null` | Find world-writeable files
`find / ! -path "*/proc/*" -perm -2 -type f -print 2> /dev/null` | Find world-writeable files excluding those in /proc
`find / -perm -2 -type d 2> /dev/null` | Find word-writeable directories
`find /home –name *.rhosts -print 2> /dev/null` | Find rhost config files
`find /home -iname *.plan -exec ls -la {} ; -exec cat {} 2> /dev/null ;` | Find *.plan files, list permissions and cat the file contents
`find /etc -iname hosts.equiv -exec ls -la {} 2> /dev/null ; -exec cat {} 2> /dev/null ;` | Find hosts.equiv, list permissions and cat the file contents
`ls -ahlR /root/` | See if you can access other user directories to find interesting files
`cat ~/.bash_history` | Show the current users’ command history
`ls -la ~/.*_history` | Show the current users’ various history files
`ls -la /root/.*_history` | Can we read root’s history files
`ls -la ~/.ssh/` | Check for interesting ssh files in the current users’ directory
`find / -name "id_dsa*" -o -name "id_rsa*" -o -name "known_hosts" -o -name "authorized_hosts" -o -name "authorized_keys" 2> /dev/null \| xargs -r ls -la` | Find SSH keys/host information
`ls -la /usr/sbin/in.*` | Check Configuration of inetd services
`grep -l -i pass /var/log/*.log 2> /dev/null` | Check log files for keywords (‘pass’ in this example) and show positive matches
`find /var/log -type f -exec ls -la {} ; 2> /dev/null` | List files in specified directory (/var/log)
`find /var/log -name *.log -type f -exec ls -la {} ; 2> /dev/null` | List .log files in specified directory (/var/log)
`find /etc/ -maxdepth 1 -name *.conf -type f -exec ls -la {} ; 2> /dev/null` | List .conf files in /etc (recursive 1 level)
`ls -la /etc/*.conf` | As above
`find / -maxdepth 4 -name *.conf -type f -exec grep -Hn password {} ; 2> /dev/null` | Find .conf files (recursive 4 levels) and output line number where the word ‘password’ is located
`lsof -i -n` | List open files (output will depend on account privileges)
`head /var/mail/root` | Can we read roots mail