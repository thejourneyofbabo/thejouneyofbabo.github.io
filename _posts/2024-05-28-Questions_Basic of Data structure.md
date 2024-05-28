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
fn main() {
	let mut vec = vec![1, 2, 3, 4, 5];
	vec.sort();
	match vec.binary_search(&3) {
		Ok(index) => println!("Found at index {}", index),
		Err(_) => println!("Not Found"),	
	}
}
```

**Trade-offs compare to Other Data Structures:**
- **HashMap:** If you need fast lookups, a **'HashMap'** offers average-case O(1) time complexity for search operations.
```rust
use std::collections::HashMap;
```
```rust
fn main() {
	let mut map = HashMap::new();
	map.insert(1, "one");
	map.insert(2, "two");
	map.insert(3, "three");
	
	if let Some(value) = map.get(&2) {
		println!("Found: {}", value);
	} else {
		println!("Not Found");
	}
}
```
*Trade-off*: Hash maps use more memory compared to vectors and have an overhead for hashing.
- **BTreeMap:** If you need a sorted map with efficient lookups, **'BTreeMap'** provides O(log n) time complexity for search operations.
```rust
use std::collections::BTreeMap;
```
```rust
fn main() {
	let mut map = BTreeMap::new();
	map.insert("apple", 3);
	map.insert("banana", 2);
	map.insert("orange", 5);

	println!("{:?}", map);

	if let Some(value) = map.get(&"banana") {
		println!("Found: {}", value);
	}
}
```





## Reference

