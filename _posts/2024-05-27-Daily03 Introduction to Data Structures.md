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
[Embedded code](https://play.rust-lang.org/?version=stable&mode=debug&edition=2021&code=fn+main%28%29+%7B%0A%09let+mut+vec+%3D+vec%21%5B1%2C+2%2C+3%2C+4%2C+5%5D%3B%0A%09println%21%28%22Original+vector%3A+%7B%3A%3F%7D%22%2C+vec%29%3B%0A%0A%09%2F%2F+Add+elements%0A%09vec.push%286%29%3B%0A%09vec.push%287%29%3B%0A%09println%21%28%22After+adding+elements%3A+%7B%3A%3F%7D%22%2C+vec%29%3B%0A%0A%09%2F%2F+Remove+elements%0A%09vec.pop%28%29%3B%0A%09println%21%28%22After+removing+element%3A+%7B%3A%3F%7D%22%2C+vec%29%3B%0A%0A%09%2F%2F+Access+elements%0A%09println%21%28%22Element+at+index+2%3A+%7B%7D%22%2C+vec%5B2%5D%29%3B%0A%0A%09%2F%2F+Modify+an+element%0A%09vec%5B2%5D+%3D+10%3B%0A%09println%21%28%22Modified+vector%3A+%7B%3A%3F%7D%22%2C+vec%29%3B%0A%7D)








## Reference
**ChatGPT_ AI coach**
