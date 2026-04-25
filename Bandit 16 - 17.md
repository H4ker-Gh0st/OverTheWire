#Bandit 
## Level Goal

The credentials for the next level can be retrieved by submitting the password of the current level to **a port on localhost in the range 31000 to 32000**. First find out which of these ports have a server listening on them. Then find out which of those speak SSL/TLS and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

**Helpful note: Getting “DONE”, “RENEGOTIATING” or “KEYUPDATE”? Read the “CONNECTED COMMANDS” section in the manpage.**

## Commands you may need to solve this level

ssh, telnet, nc, ncat, socat, openssl, s_client, nmap, netstat, ss

## Helpful Reading Material

- [Port scanner on Wikipedia](https://en.wikipedia.org/wiki/Port_scanner)

## RASPUNSUL

nmap -sV -p 31000-32000 localhost
openssl s_client -connect localhost:31790 -quiet -servername localhost <<< "kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx"
[obtinem private key , copy paste intrun file pe desktop cu terminatia .private]
ssh -i sshkey2.private bandit17@bandit.labs.overthewire.org -p 2220
[KEY stocata in /etc/bandit_pass/bandit17]

KEY : EReVavePLFHtFlFsjn3hyzMlvSuSAcRD
