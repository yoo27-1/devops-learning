## Bandit level 0

## Level Goal

The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

## Solution

In linux terminal, write the command:
ssh bandit0@bandit.labs.overthewire.org -p 2220

Then, when prompted, the password to input is bandit0.

## Explanation

The format for the ssh command goes, <username>@<remote>, then to input the specified port which in this case was 2220, the next argument would be -p <port>

## What I learned

I learned how to log into a domain using a username and password and changing the port number, through use of the SSH command in terminal.