# Level 12

## Level Goal
The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Soulation
using xxd -r to revert the hexdump file into the first compressed file.
once converted we have a train of a number differnty compression types

using file <file name> to find out the type of file then using one of the following

gzip - 
  1) mv <old file name> <new file name>.gz
  2) gzip -d <new file name>.gz (-d = decompress) 

bzip2 - 
  1) bzip2 -d <file name>

tar - 
  1) tar -xvf <file name>

once at the ASCII file cat the file



password: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
