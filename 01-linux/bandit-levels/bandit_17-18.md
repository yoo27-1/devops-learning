## Bandit level 17 - 18

## Level Goal

There are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19

## Solution

diff passwords.old passwords.new

## Explanation

diff displays the lines that are different between two files. I then copied the different line as the new password

## What I learned
How to use diff to compare the differences between two similar files