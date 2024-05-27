---
layout: single
title: HashSet_Collection of Unique values
categories:
  - Programming
tags:
  - rust
  - data_structure
aliases:
  - HashSet
connected:
  - "[[Rust]]"
toc: true
author_profile: true
---
## What is a HashSet?
A HashSet is a fundamental data structure in Rust's standard library (`std:::collections::HashSet`). It represent an unordered collection of unique values. Think of it as a bag where you can throw in items, but each item can only exist once inside.

### Key Characteristics:
1. **Uniqueness:** Guarantees the uniqueness of its elements. If you try to insert a value that already exists in the set, it will simply be ignored.
2. **Unordered:** The element within a HashSet are not stored in any particular sequence. The order you insert items might not be the order you retrieve them.
3. **Efficient Membership Testing:** Thanks to its underlying hash table implementation, HashSet excels at quickly checking whether a specific value is present within the set. This is ofter referred to as "membership testing" and is much faster than searching through a list or array.

### How does a HashSet work (Behind the scenes)?
A HashSet uses a hash function to determine where to store each element. A hash function takes an input value and produces a numerical output (a hash code) that ideally should be unique for each distinct input. This hash code is then used as an index to store or retrieve the element within the HashSet's internal storage.

### Why use a HashSet?
- **Removing Duplicates:** If you have a collection of items and you need to eliminate duplicates, a HashSet is the perfect tool.
- **Fast Lookups:** When  you need to repeatedly check if a value exists within a set, HashSet's efficient lookup is invaluable.
- **Mathematical Set Operations:** HashSets support operations like union, intersection, and difference, which are very useful in set theory and many algorithms.

### Creating and Using a HashSet:
```rust
use std::collections::HashSet;

let mut books = HashSet::new(); // Create an empty HashSet
books.insert("The Lord of the Rings");
books.insert("The Hitchhiker's Guide to the Galaxy");
books.insert("The Lord of the Rings"); // This won't be inserted again

println!("{:?}", books); // Prints the uniuqe book titles

if books.contains("The Hitchhiker's Guide to the Galaxy") {
	println!("This book is in the set!");
}
```
[Code in Playground](https://play.rust-lang.org/?version=stable&mode=debug&edition=2021&gist=ff1f7e4729b36b623a45b53197787e3d)

### HashSet Methods:
HashSet offers a rich set of methods for inserting, removing, checking membership, iterating over elements, and performing set operations. Some common ones:
- `insert(value)`: Inserts a value into the set.
- `remove(value)`: Removes a value from the set.
- `contains(value)`: Checks if a value is in the set.
- `is_empty()`: Checks if the set is empty.
- `len()`: Returns the number of elements in the set.
- `iter()`: Returns an iterator over the elements in the set.
- `union()`, `intersection()`, `difference()`: Performs set operations.







## Reference

