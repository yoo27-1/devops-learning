## Bandit level 13 - 14

## Level Goal

The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Look at the commands that logged you into previous bandit levels, and find out how to use the key for this level.
If you need help with this level: a hint file can be found in the home directory.
Make sure to read the error messages as they are informative.

## Solution

Exit bandit to local machine. Use scp command:
scp -P 2220 bandit13@bandit.labs.overthewire.org:.
Then:
cp sshkey.private ~
Then:
chmod 600 sshkey.private
Then:
ssh -i sshkey.private -p 2220 bandit14@bndit.labs.overthewire.org

## Explanation

Must make use fo scp and chmod and ssh
Return to local machine to use the scp file transfer from remote to local, the . for the path means current working directory. I then copied the key file to the home directory in order to manage permissions properly. chmod 600 makes sure the owner aka me has read and write permissions, while the group and everyone else has none, so no errors pop up. To connect to bandit14, I do the same ssh as usual instead adding an argument -i sshkey.private in order to bypass the password and use the key instead.

## What I learned
How to use scp, knowing to return to local machine to use scp, finding out you cannot change permissions effictively on wsl local machines without moving to home directory, and logging in via ssh with a key instead of a password.