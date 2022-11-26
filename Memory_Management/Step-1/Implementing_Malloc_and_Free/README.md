# Introduction
In this section, we’ll explore a simple implementation of the `malloc()` and `free()` functions used for dynamic memory allocation and deallocation.  
在本节中，我们将探索用于动态内存分配和释放的`malloc()`和`free()`函数的简单实现。  

# Representing Blocks
# 表示块
We will need a small block at the beginning of each chunk that contains extra information called **meta-data**. This block holds, at the very least:  
我们将需要每个块的开头处的一个小块，其中包含称为**元数据**的额外信息。这个块至少包含：

- A pointer to the next chunk
    指向下一个块的指针
- A flag to mark free chunks, and
    标记空闲块的标志
- The size of the data of the chunk.
    块数据的大小。

This block of information comes before the pointer returned by `malloc`
这个信息块位于`malloc`返回的指针之前

![image](../../../img/c2ad4d23fea461b5f27da451bb190f9f-22663d9559f5f029.webp)

The graphic above shows an example of heap organization with the meta-data in front of the allocated block. Each chunk of data is made of a block of metadata followed by the block of data. The pointer returned by `malloc` is shown in the lower part of the graphic. Notice that it points on the data block, not on the complete chunk.  
上图显示了带有元数据的堆组织的示例。每个数据块都由元数据块和数据块组成。`malloc`返回的指针显示在图形的下部。注意，它指向数据块，而不是完整的块。  

The metadata (data about data) is stored in a block of memory next to the specific block of allocated memory to which it belongs. This metadata block, or more specifically the linked list structure is essential because we need to know whether a given block is free or already allocated, as well as the size of the block to which it refers.  
元数据（关于数据的数据）存储在与它所属的特定分配内存块相邻的内存块中。这个元数据块，或者更具体地说，链表结构是必不可少的，因为我们需要知道给定块是否空闲或已分配，以及它所指的块的大小。  

The following is the metadata block structure:  
以下是元数据块结构：

```c
struct block{
    size_t size;
    int free;                             
    struct block *next; 
};  
```

