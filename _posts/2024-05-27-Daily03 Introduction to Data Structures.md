---
layout: single
title: Daily03 Introduction to Data Structures
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
**Definition:** Data structures are ways to store and organise data so that they can be used efficiently.

**Importance:**
- Fundamental for building efficient software.
- Help manage and process data efficiently.
- Choosing the right data structure can improve performance.

## 2. Arrays
**Definition:** An array is a fixed-size collection of elements of the same type stored in contiguous memory locations.

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
	println!("Modified array: {:?}", array);
}
```

### 3. Vectors
**Definition:** A Vector is a resizable array, which can grow or shrink in size.

**Syntax in Rust:**
```rust
fn main() {
	let mut vec: Vec<i32> = Vec::new(); // Creating an empty vector
	vec.push(1);
	vec.push(2);
	vec.push(3);
	println!("{:?}", vec);
}
```
**Key Points:**
- Dynamically sized.
- Useful when you don't know the number of elements in advance.

**Usage:** 
```rust
fn main() {
	let mut vec = vec![1, 2, 3, 4, 5];
	println!("Original vector: {:?}", vec);

	// Add elements
	vec.push(6);
	vec.push(7);
	println!("After adding elements: {:?}", vec);

	// Remove elements
	vec.pop();
	println!("After removing element: {:?}", vec);

	// Access elements
	println!("Element at index 2: {}", vec[2]);

	// Modify an element
	vec[2] = 10;
	println!("Modified vector: {:?}", vec);
}
```
[Code in Playground](https://play.rust-lang.org/?version=stable&mode=debug&edition=2021&gist=f710f4db23bea230785ee2182380490f)

### 4. Tuples

**Definition:** A tuple is a fixed-size collection of elements of potentially different types.

**Syntax in Rust**:
```rust
fn main() {
	let tuple: (i32, f64, char) = (42, 6.7, 'c'); // A tuple with different types
	println!("{:?}", tuple);
}
```

**Key Points:**
- Fixed size.
- Elements can be of different types.
- Useful for grouping together different types of values.

**Usage:**
```rust
fn main() {
	let tuple = (42, 6.7, 'c');
	let (x, y, z) = tuple; // Destructuring the tuple
	println!("The value of x is: {}", x);
	pritnln!("The value of y is: {}", y);
	println!("The value of )
}
```




## Reference
**ChatGPT_ AI coach**
