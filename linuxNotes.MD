# Linux Notes
This is where I will keep track of my daily linux practice.

## Day 1
### kill - 9 pid#

useradd - add users

/etc/passwd - shows users 
/etc/shadow - shows hashed passwords for users

# MV - move command
can change name or move directors

## Day 2 notes - networking
ping -c4 - ping out

*arp* -a - sends arp out, associates IP addresses with MAC address

> _netstat_ - shows informatino on connections

# 09/11 Notes


# CHOWN - change file owner and group information

# CHMOD - change file access permision r,w,x

> OWNER / Group / Others

## useradd - r tomcat

>chown -R tomcat:tomcat /usr/local/tomcat
>Gives permissions and ownership to Tomcat installation direction


>In Unix and Linux, a daemon is a program that runs in the background without requiring any user interaction. The file name of a software daemon usually ends in the letter d.


# net-tools - net-stat
networking stats - shows open ports, 

## netstat -nr
> shows network routing table

## netstat -ant 
> shows sockets and stats

## netstat -ai
> shows satts on network interface configed

## netstat -pnltu
> shows services and coreresponding ports

--------------------------

# NMAP 
> creates map of network by discovering host on which running.

nmap 127.0.01

or

firewall-cmd --list-ports

# 09/12 notes
*Linux everything is a file*

<li>bin - programs/binaries
<li>boot - files needed for booting
<li>etc - configuration files
<li>home - directory (cd ~)
<li>root - only root can access
<li>lib - library files, software dependenceis
<li>var - log files, 
<li>proc - running processes

ls /bin -- all programs, executables


## TOP
top -f - tells all active services running

free -f - tells all space

/proc/sys/kernel/pid_max - tells all PID running

# 09/21
Systemctl provides management for OS and services running. == OS configuration

### Systemctl is for system management and service management

> systemctl subcommand argument
systemctl restart (servicename)

systemctl reboot - reboots

### systemctl shows all active services and sattuses

systemctl list-units 
systemctl list-units --type=service --state=active

systemctl start {service_name}
systemctl stop **
systemctl restart **
systemctl disable **

systemctl mask ** (if service stoped, can also be stopped by other service, tihs prevents service from starting*)

systemctl kill ** (prefer not to kill, but diable)

## service sshd status
OR

# systemctl status sshd.service
> check status of service runnings

systemctl enable (service)
systemctl status **
service ** status

# systemctl list-unit-files
lists all services running 

# notes 09/30

## find vs locate command
find can search - . (dir), /  - whole system, or ~ - home folder
> find <location/director> <options> <search>

<li> find . -name my-file</li>
<li>find . -iname my-file</li>

## LOCATE

# 10/02

## ps - snapshot of processes
## top - show real time processes

## kill pid - kill process with id
> pkill name - will process with name
> killall name - kill all w/ names beginningq

# Notes 10/13

> A symlink is a symbolic Linux/ UNIX link that points to another file or folder on your computer, or a connected file system. This is similar to a Windows shortcut. Symlinks can take two forms: Soft links are similar to shortcuts, and can point to another file or directory in any file system.

## register redhat 
> sudo subscription-manager register --username *** --password

