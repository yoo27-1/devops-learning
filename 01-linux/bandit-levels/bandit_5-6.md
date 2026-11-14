## Bandit level 5 - 6

## Level Goal

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

    human-readable
    1033 bytes in size
    not executable

## Solution

Input the command:
find . -type f -size 1033c ! -executable
then cat the file directory outputted: 
cat ./maybehere07/.file2

## Explanation

the find command takes arguments of types, sizes, and whether it was executable as a few of the arguments available. The level requires us to find the file that has a size smaller than 1033 bytes, human readable, and not executable. type -f finds a regular file, -size 1033c finds size under 1033 bytes and ! -executable means not executable (! is for not).

## What I learned
How to find specific files that have a list of properties