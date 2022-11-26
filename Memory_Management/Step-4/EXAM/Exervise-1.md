# Virtual Memory Systems

## A dirty page is…
- modified
- corrupted
- inactive

### Answer
A dirty page is one that has been modified but not yet written to the disk via IO.


## Fill in the comparison table about VMS and Linux
| Aspect                  |           VMS           |                  Linux |
|:------------------------|:-----------------------:|-----------------------:|
| virtual address space   |  pages and segmented    | pages                  |
| page table structure    |  linear table           | four-level table       |
| page replacement policy |  FIFO with dirty/clean list | LRU with active/inavtive list |

## The biggest difference between older and newer operating systems is…  
- paged memory with swap space
- security
- lazy optimizations

### Answer
VAX/VMS had lazy optimizations and paged/swapped memory decades ago – where as the networking of computers has required OSs to become more secure.  
