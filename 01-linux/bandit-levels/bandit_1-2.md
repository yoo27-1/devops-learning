## Bandit level 1 - 2

## Level Goal

The password for the next level is stored in a file called - located in the home directory.

## Solution
Input the command cat ./- then copy the password shown.

## Explanation
Since the file is a dashed filename, which reads as the start of an option. The terminal waits for an input indefinitely, so in order to read the file you must use ./- to refer to the dashed filename.

## What I learned
How to open filenames with a dash at the beginning without there being any errors or indefinite waiting times by the terminal.