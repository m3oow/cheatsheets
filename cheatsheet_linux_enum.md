# Cheatsheet for Linux enumeration

## Table of contents
* [Kernel, OS & devices](#kernel)
* [Bash](#bash_shell)
* [Perl](#perl_shell)
* [Python](#python_shell)
* [PHP](#php_shell)
* [Netcat](#netcat_shell)
* [Telnet](#telnet_shell)

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
