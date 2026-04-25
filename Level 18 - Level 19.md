#Bandit 
## Level Goal

The password for the next level is stored in a file **readme** in the homedirectory. Unfortunately, someone has modified **.bashrc** to log you out when you log in with SSH.

## Commands you may need to solve this level

ssh, ls, cat

## RASPUNSUL

in bandit17:
cat /etc/shells
exit
ssh bandit18@bandit.labs.overthewire.org -p 2220 -t "/bin/sh"
[INPUT PASSWORD] x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
loginul este oprit prin scripturi
cat readme
KEY : cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8