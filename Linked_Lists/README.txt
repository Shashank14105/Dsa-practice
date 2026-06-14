# Linked List in Java

This directory contains a **custom-built Linked List** implementation (without Java's Collection Framework) and standalone problem files that each define their own minimal `LinkedList` class to solve a specific problem.

---

## 🔧 Core Implementation — `LinkedList.java`

All operations are built from scratch using a custom `Node` class.

| No. | Operation / Method | Description | Complexity |
|---|---|---|---|
| 1 | **`addFirst(data)`** | Insert a node at the beginning of the list | O(1) |
| 2 | **`addLast(data)`** | Insert a node at the end of the list | O(1) |
| 3 | **`add(data, index)`** | Insert a node at a specific index | O(n) |
| 4 | **`removeFirst()`** | Remove and return the first node's value | O(1) |
| 5 | **`removeLast()`** | Remove and return the last node's value | O(n) |
| 6 | **`deleteNthFromEnd(n)`** | Remove the n-th node from the end | O(n) |
| 7 | **`search(key)`** | Iteratively search for a key; return its index | O(n) |
| 8 | **`recSearch(key)`** | Recursively search for a key; return its index | O(n) |
| 9 | **`reverse()`** | Reverse the linked list in-place | O(n) |
| 10 | **`printLL()`** | Print all nodes in `data->null` format | O(n) |
| 11 | **`mergeSort(head)`** | Sort the linked list using Merge Sort | O(n log n) |

---

## 🔧 Doubly Linked List — `DoubleLL.java`

Each `Node` has both a `next` and a `prev` pointer, enabling O(1) removal from both ends.

| No. | Operation / Method | Description | Complexity |
|---|---|---|---|
| 1 | **`addFirst(data)`** | Insert at head — update `newNode.next = head` and `head.prev = newNode` | O(1) |
| 2 | **`removeFirst()`** | Remove head — move head forward, set `head.prev = null` | O(1) |
| 3 | **`removeLast()`** | Remove tail — move tail backward using `tail.prev`, set `tail.next = null` | O(1) |
| 4 | **`reverse()`** | Swap `next` and `prev` pointers for every node | O(n) |
| 5 | **`print()`** | Print nodes in `null<->data<->null` format | O(n) |

---