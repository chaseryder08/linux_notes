# LINUX COMPLTED PROJECTS

# 09/04 
- 171-[JAWS]-Lab - Creating Amazon EC2 Instances 
- 173-[JAWS]-Activity: Troubleshoot Create Instance
scripting JSON file to automate EC2 creation of LAMP stack for website.
-troubleshoot bugs in script

# 09/05 
IPSWEEPER.sh project - sweeps for active IPs on network
#!/bin/bash

if [ "$1" == "" ]
then
echo "Please enter an IP address"
echo "SYNATAX: ./ipsweeper.sh 192.168.137"

else
for ip in `seq 1 254`; do
ping -c 1 $1.$ip | grep "64 bytes" | cut -d " " -f 4 | tr -d ":" &
done
fi


