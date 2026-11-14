## Bandit level 2 - 3

## Level Goal

The password for the next level is stored in a file called --spaces in this filename-- located in the home directory

## Solution

Input the following command within the home directory:
cat ./--spaces\ in\ this\ filename--

## Explanation

The filename contains spaces. The way to counter that is to write a forward slash in between each 'word'. This allows the file to be accessed. Since it has a dash at the start, the ./ is also needed at the beginning.

## What I learned

When dealing with filenames with spaces between the words, you must use forward slashes to separate them when necessary.