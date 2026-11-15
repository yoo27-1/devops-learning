## Bandit level 11 - 12

## Level Goal

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Solution

Input command:
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

## Explanation

tr translates the text in the file to shift each character by 13. The inputs are the first argument and the outputs are the 2nd argument, both uppercase and lowercase being handled separately.

## What I learned
How to use the tr command to manipulate text in a file.