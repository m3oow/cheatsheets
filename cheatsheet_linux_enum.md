# Cheatsheet for Linux enumeration

## Table of contents
* [Kernel, OS & devices](#kernel)
* [Users & groups](#users)

## Kernel, OS & devices <a name="kernel"></a>
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

## Users & Groups <a name="users"></a>
Command | Result
------------ | -------------
`cat /etc/passwd` | List all users on the system
`cat /etc/group` | List all groups on the system
<code>for i in $(cat /etc/passwd 2> /dev/null | cut -d ":" -f1 2> /dev/null); do id $i; done 2> /dev/null</code> | List all uid’s and respective group memberships
`cat /etc/shadow` | Show user hashes – Privileged command
<code>grep -v -E "^#" /etc/passwd | awk -F: '$3 == 0 { print $1}'</code> | List all super user accounts
`finger` | Users currently logged in
`pinky` | As above
`users` | As above
`who -a` | As above
`w` | Who is currently logged in and what they’re doing
`last` | Listing of last logged on users
`lastlog` | Information on when all users last logged in
`lastlog –u %username%` | Information on when the specified user last | logged in
`lastlog | grep -v "Never"` | Entire list of previously logged on users

## User & Privilege Information <a name="privileges"></a>
Command | Result
------------ | -------------
`whoami` | Current username
`id` | Current user information
`cat /etc/sudoers` | Who’s allowed to do what as root – Privileged command
`sudo -l` | Can the current user perform anything as root
`sudo -l 2>/dev/null | grep -w 'nmap'|'perl'|'awk'|'find'|'bash'|'sh'|'man'|'more'|'less'|'vi'|'vim'|'nc'|'netcat'|'python'|'ruby'|'lua'|'irb' | xargs -r ls -la 2>/dev/null` |	Can the current user run any ‘interesting’ binaries as root and if so also display the binary permissions etc.