# Level 16
## Level Goal
ls for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

## Soulation
using the nmap command to scan the required port range to find any open ports

```nmap -sT -p 31000-32000 localhost```

Then with the ports that are open check to see which ports have ssl enabled

```nmap --script +ssl-cert -p 31046-31960 localhost```
nmap comes with a number of scripts the one being used lists details about ports with ssl enable by
default the above command will only scan a hand full of pre-defind port using the ```+``` lets
the command scan any port. 

password: a private key in the file key
