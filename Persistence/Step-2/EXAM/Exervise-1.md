# Exercise 1
Write a program that reads and prints the contents of a directory, similar to the ls command. This program should:  
- Accept a directory name as input
- Loop repeatedly, reading one directory entry at a time
- Print out the inode number and name of each file in the directory.

Your output should look similar to the output below:

```bash
52 .
66 ..
154 .guides
1249 .settings
519 myls.c
8616 myls
```

```c src.c
#include <sys/types.h>
#include <sys/stat.h>
#include <unistd.h>
#include <stdio.h>
#include <stdlib.h>
#include <dirent.h>

int main(int argc, char* argv[])
{
    // YOUR CODE HERE
}
```