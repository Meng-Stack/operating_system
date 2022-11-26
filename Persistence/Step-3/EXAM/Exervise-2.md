# Exercise 2

## Question 1
Log-structured file systems were created to deal with **increasing disk sizes, inefficient reading and writing**, and **file systems that lacked RAID awareness**.

## Question 2
- **Segment Usage Table**: shows how much data is on each block.
- **Inode Map**: This shows where each inode on the disk is located. This is written directly into the segment.
- **Segment Summary**: This keeps track of the details for each block in the segment.
- **Inodes**: These carry physical block pointers to files.