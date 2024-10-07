# Matching paths with []

## Procedure
I started the challenge, I connected the terminal.<br>
i went to `/home/hacker` directory, and then typed `/challenge/challenge /challenge/files/file[bash]`
and i got the flag, i pasted it into my flag box.

## bash
`Connected!
hacker@globbing~matching-paths-with-:~$ cd /challenge/files
hacker@globbing~matching-paths-with-:/challenge/files$ ls
file_a  file_d  file_g  file_j  file_m  file_p  file_s  file_v  file_y
file_b  file_e  file_h  file_k  file_n  file_q  file_t  file_w  file_z
file_c  file_f  file_i  file_l  file_o  file_r  file_u  file_x
hacker@globbing~matching-paths-with-:/challenge/files$ /challenge/run /home/hacker/file_[bash]
Error: please run with a working directory of /home/hacker!
hacker@globbing~matching-paths-with-:/challenge/files$ /challenge/run /challenge/files/file_[bash]
Error: please run with a working directory of /home/hacker!
hacker@globbing~matching-paths-with-:/challenge/files$ cd /home/hacker
hacker@globbing~matching-paths-with-:~$ ls
a  flag  not-the-flag
hacker@globbing~matching-paths-with-:~$ ls -a
.   .bash_history  .bashrc   .profile  flag
..  .bash_logout   .lesshst  a         not-the-flag
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{EKmXAD5jkBPhk8TPsj-BNkwWPzB.dRjM4QDLyIDO0czW}`

## Reference
Didnt use
