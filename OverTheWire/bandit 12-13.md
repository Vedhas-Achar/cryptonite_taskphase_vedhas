# bandit 12-13

## Procedure
i connected my terminal, then i used `cp data.txt /tmp/challenge` to copy it 
into the `/challenge` directory , then i used `xxd -r data.txt > data` and then
used `file data` to get to know its type, then it was `gzip` file, hence i changed 
its name into gzip using `mv data file.gz` and then used `gzip -d file.gz` and then 
got its decompressed form in a different file type, i continued to rename it and 
decompress it until it became into an ASCII file, then i read it, which i got the password.

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
Friends , copilot , chatgpt
