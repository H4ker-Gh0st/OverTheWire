#Bandit 
## Level Goal

The password for the next level is stored in **/etc/bandit_pass/bandit14 and can only be read by user bandit14**. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Look at the commands that logged you into previous bandit levels, and find out how to use the key for this level.

## Commands you may need to solve this level

ssh, scp, umask, chmod, cat, nc, install

## Helpful Reading Material

- [SSH/OpenSSH/Keys](https://help.ubuntu.com/community/SSH/OpenSSH/Keys)

## RASPUNSUL

scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.private C:\Users\mortifer\Desktop
ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
cat /etc/bandit_pass/bandit14

KEY: MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS