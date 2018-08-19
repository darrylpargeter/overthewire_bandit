### Level 6

## Level Goal
The password for the next level is stored somewhere on the server and has all of the following properties:

    owned by user bandit7
    owned by group bandit6
    33 bytes in size

## Soulation
find / -group bandit6 -user bandit7 -size 33c 2>/dev/null
password: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs 
