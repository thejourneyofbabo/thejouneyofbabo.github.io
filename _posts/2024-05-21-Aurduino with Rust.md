---
layout: single
title: Aurduino with Rust
categories:
  - Embedded Rust
tags:
  - embedded
  - rust
  - arduino
toc: true
author_profile: true
aliases:
  - Arduino with Rust
connected:
  - "[[2024-05-21-'uno-blink'_Rust|uno-blink]]"
---
## How to start?
["avr-hal"_github link_](https://github.com/Rahix/avr-hal)
Following the link, the github repository of 'avr-hal'. Embedded-hal abstractions for AVR microcontrollers

### Examples
`cd examples/arduino-uno/src/bin` 
At this folder, we can find multiple example code by using Rust for Arduino.
ex) "uno-16chan-servo-drivers.rs"

### How can run the examples?
```
# Build and run in on a connected board
cargo run --bin uno-blink
```

## What I will do
- Understanding how the Rust code works with Arduino
- Build my own Rust-Arduino(microcontroller) project
	- Rust_arduino_car
- Let's have a look
