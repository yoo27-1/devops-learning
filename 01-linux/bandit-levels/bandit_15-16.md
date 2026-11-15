## Bandit level 15 - 16

## Level Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL/TLS encryption.

## Solution

openssl s_client -connect localhost:30001
then paste the current password to return the level 16 password

## Explanation

Instead of telnet, in order to wrap it in SSL/TLS encryption, the openssl s_client command must be used. It is the same process as before except for that

## What I learned
The command to wrap SSL/TLS encryption when connecting to localhost
