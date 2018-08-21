# Level 13
## Level Goal
The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

## Soulation
using the ssh command and the -i flag
The -i is the identy flag and can be passed a private key
```ssh -i sshkey.private bandit14@localhost```
then cat the file located at /etc/bandit_pass/bandit14
password: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
