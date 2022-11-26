# Exercise 1
Write a program that implements the First Come First Serve disk scheduling algorithm. This program should:  

- Prompt the user to enter   10  disk locations to service   (0−199) 
- Access each request in the order they were received
- The disk head should start on sector   10 
- Calculate the total movement of the disk head
- Print the requests in the order they’re serviced
- Print the total movement of the disk head

Your output should look like this:

```bash
Enter disk locations to service: 95 30 78 187 5 81 169 65 15 73
Sector 95
Sector 30
Sector 78
Sector 187
Sector 5
Sector 81
Sector 169
Sector 65
Sector 15
Sector 73
Total Disk Head Movement: 865
```

```c src.c
#include<stdio.h>
#include<stdlib.h>

int main(int argc, char *argv[])
{
    // YOUR CODE HERE
   return 0;
}
```