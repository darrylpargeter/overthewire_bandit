# Level 15

## Level Goal
The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.

## Soulation
Like level 14 we need to use a commond that close resembals netcat
the ```openssl``` command handles the ssl/tls side of things
and ```s_client``` dose the connection to the server.

-ign_eof - inhibit shutting down t econnection when end of file is reached in the input

using the following
```openssl s_client -ign_eof localhost:30001```
then pasting the level 14 password

password: cluFn7wTiGryunymYOu4RcffSxQluehd 
