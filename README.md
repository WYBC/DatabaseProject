# DatabaseProject
Database Project for CPSC 437 final. Can eventually tie in to 2015 site project.

## Access:
ssh -i <key> ec2-user@52.91.177.0

## bashrc
sudo vim /etc/bashrc
change this line to:
[ "$PS1" = "\\s-\\v\\\$ " ] && PS1="\[\e[0;36m\]$NICKNAME:\[\e[m\] \[\e[1;31m\]\W\[\e[0m\] > "
