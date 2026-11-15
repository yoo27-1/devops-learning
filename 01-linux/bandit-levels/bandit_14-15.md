## Bandit level 14 - 15

## Level Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

## Solution

in bandit14,
cd /etc/bandit_pass
cat bandit14
Gives password for level 14, then:
telnet localhost 30000
input password for level 14
then password for level 15 is given.

## Explanation

telnet opens a connection to localhost through port 30000, which is what the level goal requires. It needed the password for current level, and the previous level said it was stored in /etc/bandit_pass/bandit14, which is where I checked. After connecting through telnet, I pasted the password and the next password was given.

## What I learned
Basics of telnet