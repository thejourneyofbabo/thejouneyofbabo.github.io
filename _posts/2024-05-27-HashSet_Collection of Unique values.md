---
layout: single
title: HashSet_Collection of Unique values
categories:
  - Daily Study
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
A HashSet uses a hash function to determine where to store each element. A hash function takes an input value and produces a









## Reference

