# Max Heap Implementation

This project implements a Max Heap data structure using a binary tree represented as an array. The Max Heap operations are defined in C++ and include methods for insertion, deletion, and maintaining heap properties.

## Overview

A Max Heap is a complete binary tree where each parent node is greater than or equal to its child nodes. This project provides a full implementation of a Max Heap, including operations to manage and manipulate the heap efficiently.

## File Structure

- **`maxh.h`**: Header file defining the `IMAXH` class with the heap operations and data members.
- **`maxh.cpp`**: Implements the methods declared in `maxh.h`.
- **`main-maxh.cpp`**: Command-line interface for interacting with the Max Heap.

## Class: `IMAXH`

The `IMAXH` class encapsulates all the functionalities related to the Max Heap. It provides methods to insert elements, delete the maximum element, print the heap, and more.

### Methods

- **Constructor & Destructor**
  - `IMAXH(int nmax = 15)`: Initializes a Max Heap with a specified capacity.
  - `~IMAXH()`: Frees the allocated memory.

- **Heap Operations**
  - `void insert(int item)`: Inserts an item into the heap.
  - `void print_max()`: Prints the maximum item in the heap.
  - `void print()`: Prints all items in the heap in a tree-like structure.
  - `void dim()`: Prints the number of items currently in the heap.
  - `void dim_max()`: Prints the maximum capacity of the heap.
  - `void clear()`: Clears all items in the heap.
  - `void deleteMax()`: Removes the maximum item from the heap.
  - `void heapify(int i)`: Restores the heap property by moving elements down.
  - `void buildMaxHeap()`: Constructs a Max Heap from the current array of elements.
  - `void redim_max(int newNv)`: Resizes the heap to a new capacity.
  - `void heapify_up(int i)`: Restores the heap property by moving elements up.

## Usage

### Building the Project

To compile the project, use the following commands:

```bash
g++ -c maxh.cpp -o maxh.o
g++ -c main-maxh.cpp -o main-maxh.o
g++ maxh.o main-maxh.o -o maxh
```

### Running the Program

Execute the following command to run the program:

./maxh


You can then enter commands to interact with the Max Heap. Available commands are:

insert <item>: Insert an item into the heap.
print_max: Print the maximum item in the heap.
print: Print all items in the heap.
dim: Print the number of items in the heap.
dim_max: Print the maximum capacity of the heap.
clear: Clear all items in the heap.
delete: Remove the maximum item from the heap.
heapify_up: Restore heap property by moving items up.
redim_max <new_capacity>: Resize the heap to a new capacity.


### Command Examples

insert 10 20 15
print_max       # Output: Max= 20
print           # Output: Heap= 20 15 10
delete          # Removes 20
print           # Output: Heap= 15 10
dim             # Output: Heap has 2 items
redim_max 30    # Resizes the heap to a new capacity

### Code Explanation

maxh.h: Defines the IMAXH class, including its data members and method declarations.
maxh.cpp: Implements the heap operations defined in maxh.h, including insertion, deletion, and heap adjustments.
main-maxh.cpp: Provides a command-line interface for interacting with the heap and processing user commands.

### Conclusion
This project provides a robust implementation of a Max Heap in C++, allowing efficient management of heap elements through various operations. The command-line interface facilitates easy interaction and testing of the heap functionalities.

### Author
Bruno Ricardo de Sá Ferreira




