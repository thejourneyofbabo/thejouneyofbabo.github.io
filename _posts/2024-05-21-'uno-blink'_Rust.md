---
layout: single
title: 2024-05-21-'uno-blink'_Rust
categories:
  - Embedded Rust
tags:
  - arduino
  - embedded
  - rust
aliases:
  - uno-blink
connected: 
toc: true
author_profile: true
---
## Code preview
>"Hello World" of the embedded programming
```rust


```

```rust
/*
* Blink the builtin LED - the "Hello World" of the embedded programming
*/
#![no_std]
#![no_main]

use panic_halt as _;

#[arduino_hal::entry]
fn main() -> ! {
	let dp = arduino_hal::Peripherals::take().unwrap();
	let pins = arduino_hal::pins!(dp);

	// Digital pin 13 is also connected to an onboard LED marked "L"
	let mut led = pins.d13.into_output();
	led.set_high();

	loop {
		led.toggle();
		arduino_hal::delay_ms(100);
		led.toggle();
		arduino_hal::delay_ms(100);
		led.toggle();
		arduino_hal::delay_ms(100);
		led.toggle();
		arduino_hal::delay_ms(100);
	}
}
```





### Reference
---
[examples/arduino-uno/src/bin/uno-blink.rs](https://github.com/Rahix/avr-hal/blob/main/examples/arduino-uno/src/bin/uno-blink.rs)
