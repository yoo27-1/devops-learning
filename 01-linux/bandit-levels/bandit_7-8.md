## Bandit level 7 - 8

## Level Goal

The password for the next level is stored in the file data.txt next to the word millionth

## Solution

Input the command:
grep -w millionth data.txt

## Explanation

grep command searches for patterns in files. the -w argument checks for matching whole words, which I used millionth for. It then gave me the line where millionth is next to the password.

## What I learned
Basic grep usage.