# Exercise 3
Write a program that implements the C-LOOK disk scheduling algorithm. This program should:  

- Prompt the user to enter   10  disk locations to service   (0−199) 
- The disk head should start on sector   10  and move toward sector   199 
- The head responds to each request in the direction it is going, until all requests are handled.
- Calculate the absolute distance of the tracks from the head.
- This distance adds to the total seek count.
- If we reach the final request in the current direction, reverse direction and move the head all the way to the location of the last request in this direction.
- Move the head in the initial direction, servicing requests until all have been completed.

Your output should look like this:

```bash
Enter disk locations to service: 95 30 78 187 5 81 169 65 15 73
Sector 15
Sector 30
Sector 65
Sector 73
Sector 78
Sector 81
Sector 95
Sector 169
Sector 187
Sector 5
Total Disk Head Movement: 359
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