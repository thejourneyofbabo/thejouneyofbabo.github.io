---
layout: single
title: Questions_Basic of Data structure
categories:
  - Programming
tags:
  - rust
  - data_structure
aliases: 
connected:
  - "[[Rust]]"
  - "[[Algorithms]]"
toc: true
author_profile: true
---
## Q1. How can I efficiently search for an element in vector, and what are the trade-offs compared to using other data structure?
**Efficient Search in a Vector:**
- **Linear Search:** This is the simplest method where you iterate through each element in the vector until you find the target. It has a time complexity of O(n).
```rust
fn main() {
	let vec = vec![1, 2, 3, 4, 5];
	let target = 3;
	if vec.contains(&target) {
		println!("Found {}", target);	
	} else {
		println!("Not Found");
	}
}
```
- **Binary Search:** If the vector is sorted, you can use binary search which has a time complexity of O(log n). Rust provides the **'binary_search'** method for vectors.
```rust
for 
```







## Reference

