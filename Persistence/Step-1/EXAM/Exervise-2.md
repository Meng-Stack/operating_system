# Exercise 2
Write a program that implements the SCAN disk scheduling algorithm. This program should:  

- Prompt the user to enter   10  disk locations to service   (0−199) 
- The disk head should start on sector   10  and move toward sector   0 
- Sort the requests from smallest to largest
- Find the current location of the disk head and move toward sector   0 , servicing requests along the way
- Switch direction at   0  and move toward higher requests, servicing until all are finished
- Calculate the total movement of the disk head
- Print the requests in the order they’re serviced
- Print the total movement of the disk head

Your output should look like this:

```bash
Enter disk locations to service: 95 30 78 187 5 81 169 65 15 73
Sector 5
Sector 15
Sector 30
Sector 65
Sector 73
Sector 78
Sector 81
Sector 95
Sector 169
Sector 187
Total Disk Head Movement: 197
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