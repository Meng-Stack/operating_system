# Exercise 1

## Question 1
A **File System Consistency Checker** is used by older Linux-based systems to find and repair inconsistencies. This method is not perfect, as it may still have **inodes** pointing to **garbage data**.  

## Question 2
- **Inode Link Checks**: FSCK counts and updates inode links. Unallocated inodes are moved to the lost and found directory.
- **Duplicate Pointers**: FSCK checks for duplicate pointers. If two inodes point to the same data block, one can be erased.
- **Free Block Checks**: FSCK scans inodes to check that blocks are tagged allocated or free.
- **Directory Checks**: FSCK checks the directory format. They should start with . and ..
- **Superblock Checks**: FSCK checks the file size against the number of blocks allocated. It looks for the questionable block and substitutes a copy.
- **Bad Blocks**: A bad pointer points to an out-of-range memory address. FSCK then deletes the pointer.
- **Inode State Checks**: FSCK checks inodes for corruption. Inodes that are corrupted are removed.