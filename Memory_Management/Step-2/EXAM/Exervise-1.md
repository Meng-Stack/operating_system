# Summative Assessment

## **Given the following information**:

- A virtual memory has a page size of 1k (1024) words.
- There are 8 pages.
- There are 4 blocks.
- The memory page table contains the information below:

| Page | Block |
|:------|:-------:|
|0	|3|
|1	|1|
|4	|2|
|6	|0|

## **Select all of the following address ranges that will result in a page fault.**  

**Hint**: Page faults occur on page numbers not specified in the memory page table. Calculate the address range by using the page of **1024** words.  

Page faults will occur on pages 2, 3, 5, and 7, which are not in the memory page table. Since each page size is 1024 words, these pages correspond to the following address ranges:

- 2048 - 3071
- 3072 - 4095
- 5120 - 6143
- 7168 - 8191