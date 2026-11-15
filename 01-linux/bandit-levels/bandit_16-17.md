## Bandit level 16 - 17

## Level Goal

The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL/TLS and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

## Solution

nmap -p 31000-32000 localhost
openssl s_client localhost:31790 -quiet
Copy the private key, logout and nano a private key file and paste the contents. Change permissions and then use ssh to log into bandit17 with that private key.

## Explanation

First command scans in the ports ranging between 31000-32000. Returned 5 ports. I then did the openssl s_client command on each port and found that 31790 was the one that didnt repeat bandit16's key back. I had to use -quiet to stop KEYUPDATE, and then doing so on port 31790 it gave the contents of a public key which I copied and logged out with to access bandit17.

## What I learned
nmap, port scanning, -quiet command