## Bandit level 12 - 13

## Level Goal

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Solution

First use mktemp -d to make a new directory within temp to decompress the files in. Then copy data.txt to the temp directory, then do xxd -r data.txt to a new file called data3.txt for example. I then did file on this file to see what compression it is. If it is gzip, then I used mv to rename the extension to gz, then gzip -d <filename>. If it was bzip2, mv to <filename>.bz2, then bzip2 -d <filename>. If it was POSIX, then tar xf <filename>. This was repeated until file <filename> said it was ASCII, which was then the password.

## Explanation

I had to make use of first reversing the hexdump, then continuously decompressing the file over and over until there was readable text at the end. 

## What I learned
How to use xxd, tar xf, bzip2, and gzip to decompress files.