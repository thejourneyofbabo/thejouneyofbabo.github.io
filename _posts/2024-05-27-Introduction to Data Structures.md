---
layout: single
title: Introduction to Data Structures
categories:
  - Programming
tags:
  - rust
  - data_structure
aliases:
  - 러스트 자료구조
  - rust data structure
connected:
  - "[[Rust]]"
  - "[[2024-05-27-HashSet_Collection of Unique values|HashSet]]"
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

## 3. Vectors
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

## 4. Tuples

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
	println!("The value of y is: {}", y);
	println!("The value of z is: {}", z);

	// Access elements by index
	println!("First element: {}", tuple.0);
	println!("Second element: {}", tuple.1);
	println!("Third element: {}", tuple.2);
}
```
[Code in Playground](https://play.rust-lang.org/?version=stable&mode=debug&edition=2021&gist=8c97efbc4e58e034c70877a9bde5c051)

## 5. Practical Examples
### **Example 1: Sum of  Array Elements**
```rust
fn main() {
	let array: [i32; 5] = [1, 2, 3, 4, 5];
	let sum: i32 = array.iter().sum();
	println!("Sum of array elements: {}", sum);
}
```
### **Example 2: Find Maximum in a Vector**
```rust
fn main() {
	let vec = vec![10, 20, 5, 15];
	let max = vec.iter().max().unwrap();
	println!("Maximum value in the vector: {}", max);
}
```
### Example 3: Tuple Operations
```rust
fn main() {
	let person: (&str, i32, f64) = ("Alice", 30, 65.5);
	println!("Name: {}", person.0);
	println!("Age: {}", person.1);
	println!("Weight: {}", person.2);
}
```
## 6. Exercises
### Exercise 1: Implement an array and print its elements.
```rust
fn main() {
	let array: [i32; 5] = [1, 2, 3, 4, 5];
	for elem in array.iter() {
		println!("{}", elem);
	}
}
```
### Exercise 2: Create a vector, add elements, and print its length.
```rust
fn main() {
	let mut vec = vec![10, 20, 30];
	vec.push(40);
	vec.push(50);
	println!("Vector legth: {}", vec.len());
}
```
### Exercise 3: Create a tuple, access and print each element.
```rust
fn main() {
	let data = ("Rust", 2024, 3.14);
	println!("Language: {}", data.0);
	println!("Year: {}", data.1);
	println!("Value: {}", data.2);
}
```




## Reference
**ChatGPT_ AI coach**
