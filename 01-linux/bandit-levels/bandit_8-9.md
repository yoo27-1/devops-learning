## Bandit level 8 - 9 

## Level Goal

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

## Solution

Make use of sort and uniq
Input:
sort data.txt | uniq -u

## Explanation

This command sorts and displays lines in the data.txt file that appear only once, which is the password in this case.

## What I learned
How to use sort and uniq to display unique lines of text within a file.