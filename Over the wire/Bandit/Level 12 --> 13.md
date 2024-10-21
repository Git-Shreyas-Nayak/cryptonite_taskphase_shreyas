# Level 12 --> 13

## Procedure
i started the challenge by reading in OverTheWire.
then i went to the terminal and connected to it.
by putting ` ssh bandit12@bandit.labs.overthewire.org -p 2220`
and password as `7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4`
then i typed `cp data.txt /tmp/challenge` to copy it .
then i went inside using cd cmd.
after that i used `xxd -r data.txt > data` this is to hexdump the file into data.
so when i use `file data` i et to know the file type .
then i renamed the file by `mv data file.gz` and gziped it by `gzip -d file.gz`.
then saw the file type again.
hence i used `mv file file.bz2` and `bzip2 -d file.bz2` to bzip the file .
i did gzip again to get tar and used this to tar out `tar xf file.tar`.
after doing this again and again untill u get to file type ASCII.
now see the file contents `cat data`.
then i noted the password `FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn`.
after that i typed exit to get of the shell.

## bash
`bandit12@bandit:~$ cp data.txt /tmp/challenge
bandit12@bandit:~$ cd /tmp/challenge
bandit12@bandit:/tmp/challenge$ ls
data  data.tar  data.txt
bandit12@bandit:/tmp/challenge$ xxd -r data.txt > data
bandit12@bandit:/tmp/challenge$ ls
data  data.tar  data.txt
bandit12@bandit:/tmp/challenge$ file data
data: gzip compressed data, was "data2.bin", last modified: Thu Sep 19 07:08:15 2024, max compression, from Unix, original size modulo 2^32 574
bandit12@bandit:/tmp/challenge$ mv data file.gz
bandit12@bandit:/tmp/challenge$ gzip -d file.gz
bandit12@bandit:/tmp/challenge$ file file
file: bzip2 compressed data, block size = 900k
bandit12@bandit:/tmp/challenge$ mv file file.bz2
bandit12@bandit:/tmp/challenge$ bzip2 -d file.bz2
bandit12@bandit:/tmp/challenge$ ls
data.tar  data.txt  file
bandit12@bandit:/tmp/challenge$ file file
file: gzip compressed data, was "data4.bin", last modified: Thu Sep 19 07:08:15 2024, max compression, from Unix, original size modulo 2^32 20480
bandit12@bandit:/tmp/challenge$ mv file file.gz
bandit12@bandit:/tmp/challenge$ gzip -d file.gz
bandit12@bandit:/tmp/challenge$ ls
data.tar  data.txt  file
bandit12@bandit:/tmp/challenge$ file file
file: POSIX tar archive (GNU)
bandit12@bandit:/tmp/challenge$ mv file file.tar
bandit12@bandit:/tmp/challenge$ tar xf file.tar
bandit12@bandit:/tmp/challenge$ file file
file: cannot open file' (No such file or directory)
bandit12@bandit:/tmp/challenge$ ls
data5.bin  data.tar  data.txt  file.tar
bandit12@bandit:/tmp/challenge$ file data5.bin
data5.bin: POSIX tar archive (GNU)
bandit12@bandit:/tmp/challenge$ mv data5.bin data.tar
bandit12@bandit:/tmp/challenge$ tar xf data.tar
bandit12@bandit:/tmp/challenge$ ls
data6.bin  data.tar  data.txt  file.tar
bandit12@bandit:/tmp/challenge$ file data6.bin
data6.bin: bzip2 compressed data, block size = 900k
bandit12@bandit:/tmp/challenge$ mv data6.bin data.bz2
bandit12@bandit:/tmp/challenge$ bzip -d data.bz2
Command 'bzip' not found, but there are 21 similar ones.
bandit12@bandit:/tmp/challenge$ bzip2 -d data.bz2
bandit12@bandit:/tmp/challenge$ ls
data  data.tar  data.txt  file.tar
bandit12@bandit:/tmp/challenge$ file data
data: POSIX tar archive (GNU)
bandit12@bandit:/tmp/challenge$ mv data data.tar
bandit12@bandit:/tmp/challenge$ tar xf data.tar
bandit12@bandit:/tmp/challenge$ ls
data8.bin  data.tar  data.txt  file.tar
bandit12@bandit:/tmp/challenge$ file data8.bin
data8.bin: gzip compressed data, was "data9.bin", last modified: Thu Sep 19 07:08:15 2024, max compression, from Unix, original size modulo 2^32 49
bandit12@bandit:/tmp/challenge$ mv data8.bin data.bz2
bandit12@bandit:/tmp/challenge$ bzip2 -d data.bz2
bzip2: data.bz2 is not a bzip2 file.
bandit12@bandit:/tmp/challenge$ ls
data.bz2  data.tar  data.txt  file.tar
bandit12@bandit:/tmp/challenge$ mv data.bz2 data.gz
bandit12@bandit:/tmp/challenge$ gzip -d data.gz
bandit12@bandit:/tmp/challenge$ file data
data: ASCII text
bandit12@bandit:/tmp/challenge$ cat data
The password is FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn`

## Reference
copilot 
