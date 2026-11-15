## Bandit level 20 - 21

## Level Goal

There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

NOTE: Try connecting to your own network daemon to see if it works as you think

## Solution

Open two terminals. Both are logged into bandit20. 
Terminal 1:
./suconnect 45000
Terminal 2:
nc -l 45000
In terminal 2, paste level 20 password.

## Explanation

Terminal 1 must execute the binary, in any port number lets say 45000. 
./suconnect 45000
Then on terminal 2, use nc to listen and connect the ports together.
nc -l 45000
Once these two are connected, I pasted the Level 20 password on terminal 2, it then was a success and returned Level 21's password.

## What I learned
How to connect two terminals together on the same port with nc and listen for certain text from one or the other.