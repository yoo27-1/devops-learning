## Bandit level 6 - 7

## Level Goal

The password for the next level is stored somewhere on the server and has all of the following properties:

    owned by user bandit7
    owned by group bandit6
    33 bytes in size

## Solution

Move to the root directory, then input the command: 
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
Then cat the directory it outputs:
cat /var/lib/dpkg/info/bandit7.password

## Explanation

The key part is 'somewhere on the server'. I made sure to move back to the root directory / before doing the find command. The properties were:
User bandit7, group bandit6, and 33 bytes in size. Those were the 3 properties I included for the arguments for my find command. I then added 2>dev/null, since it gave me many permission denied and error messages. 2 is the number for error codes, so that line makes sure all the error codes are discarded, giving me the only directory which I then used cat on and copied the password.

## What I learned
How to get rid of error codes when finding a file, searching the server, and searching by group and user ownership.