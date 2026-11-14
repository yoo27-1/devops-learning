## Bandit level 9 - 10

## Level Goal

The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

## Solution

Input command: 
strings -e s data.txt | grep -w "=="

## Explanation

The first part of the command, strings, outputs all the text in the file that is within 7 bit encoding, 's. This is ASCII. The pipe then connects the next command which finds lines that have several = within it.

## What I learned
How to use the strings command.