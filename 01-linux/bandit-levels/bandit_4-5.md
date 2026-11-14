## Bandit level 4 - 5

## Level Goal

The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

## Solution

Input the command: 
find ./*
Then cat the file that is ASCII text, then copy the password.

## Explanation

fiile ./* searches each file in  the directory and outputs what type of data it has. For most of them, it says data since there is unreadable data being outputted when using cat on the files. -file07 is the file that stored ASCII text, which was the password

## What I learned

How to search for a file that stores a specific data type