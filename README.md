# ADS
# Custom Data Structures in Java

## Overview

This project is a custom implementation of fundamental data structures in Java without using `java.util.*` (except `Iterator`). It includes:

- `MyArrayList` — dynamic array
- `MyLinkedList` — doubly linked list
- `MyStack` — stack (LIFO, built on MyArrayList)
- `MyQueue` — queue (FIFO, built on MyLinkedList)
- `MyMinHeap` — min-heap (built on MyArrayList)

## Interface

All list-based structures implement a custom interface `MyList<T>` with the following methods:

- `void add(T item)`
- `void add(int index, T item)`
- `T get(int index)`
- `T remove(int index)`
- `void set(int index, T item)`
- `int size()`
- `Iterator<T> iterator()`

## Classes Overview

### MyArrayList<T>
- Uses a resizable array internally.
- Grows when capacity is full.
- All methods implemented from `MyList`.

### MyLinkedList<T>
- Doubly linked list with head and tail.
- Inner class `MyNode<T>` with `prev`, `next` references.
- Prevents loops and supports bidirectional traversal.

### MyStack<T>
- Last-In-First-Out (LIFO) behavior.
- Based on `MyArrayList`.
- Methods: `push`, `pop`, `peek`.

### MyQueue<T>
- First-In-First-Out (FIFO) behavior.
- Based on `MyLinkedList`.
- Methods: `enqueue`, `dequeue`, `peek`.

### MyMinHeap<T extends Comparable<T>>
- Maintains a binary min-heap using `MyArrayList`.
- Methods: `add`, `getMin`, `removeMin`, `heapify`.

## Usage

Run `Main.java` to execute unit tests for all classes. Each structure is tested with valid operations and assertions.

## Development Guidelines

- Minimum of 5 commits on GitHub.
- `.gitignore` included.
- Each class documented with comments.
- Code is modular and clean.

## Author

Created by Bitimbay Rinat, BDA-2407 
Astana IT University, 2025

## License

This project is open for academic and personal use
