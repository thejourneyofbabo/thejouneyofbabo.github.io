---
layout: single
title: Daily02 Introduction to Data Structures
categories:
  - Daily Study
tags:
  - rust
  - data_structure
aliases:
  - 러스트 자료구조
  - rust data structure
connected:
  - "[[Rust]]"
toc: true
author_profile: true
---
## 1. Introduction to Data Structures
**Definition:** <br/>
Data structures are ways to store and organise data so that they can be used efficiently.

**Importance:**
- Fundamental for building efficient software.
- Help manage and process data efficiently.
- Choosing the right data structure can improve performance.

## 2. Arrays
**Definition:**<br/>
An array is a fixed-size collection of elements of the same type stored in contiguous memory locations.

**Syntax in Rust:**
```rust
fn main() {
	let array: [i32; 5] = [1, 2, 3, 4, 5]; // An array of 5 integers
	println!("{:?}", array);
}
```
**Key Points:**
- Fixed size.
- All elements must me of the same type.
- Indexing starts from 0.
**Usage:**
```rust
fn main() {
	let mut array: [i32; 5] = [1, 2, 3, 4, 5];
	println!("Element at index 2: {}", array[2]);

	// Modify an element
	array[2] = 10;
}
```






## Reference
**ChatGPT_ AI coach**
