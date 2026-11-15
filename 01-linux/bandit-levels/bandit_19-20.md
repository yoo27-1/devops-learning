## Bandit level 19 - 20

## Level Goal

To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

## Solution

./bandit20-do cat /etc/bandit_pass/bandit20

## Explanation

Running the command allows me to simulate the euid of bandit20, so I am able to access files I wasn't able to before. By executing the file and then doing a cat on the password file, I was able to do it due to having permissions

## What I learned
How to execute files and use setuid binary.