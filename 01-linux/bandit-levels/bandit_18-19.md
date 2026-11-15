## Bandit level 18 - 19

## Level Goal

The password for the next level is stored in a file readme in the homedirectory. Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

## Solution

ssh -p 2220 bandit18@bandit.labs.overthewire.org "cat readme"

## Explanation

Since it logs out instantly, I must use the speech marks in order to do all the commands at once so I can read the readme file before the logout, giving me the answer

## What I learned

Using speech marks to combine commands in one line