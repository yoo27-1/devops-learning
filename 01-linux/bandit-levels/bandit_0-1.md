## Bandit level # - #

## Level Goal

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

## Solution

I used ls to see if the readme file was in the home directory of bandit0. I then did cat readme, in order to read the file and copy the password. I then did the command exit to leave the bandit0 user, then I redid the SSH command login with the user bandit1 instead. I then pasted the password, which has been logged in the bandit-passwords.md file in the repository.

## Explanation
This level makes use of the cat command, exit command, and essentially redoes Level 0 with just a new username and a password I had to find within the readme file through terminal

## What I learned
Efficent use of the cat command.