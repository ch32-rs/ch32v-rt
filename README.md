# DEPRECATED - replaced by qingke-rt <https://github.com/ch32-rs/qingke>

# ch32v-rt

Runtime support for WCH's 32bit RISC-V MCUs.

## Usage

```rust
#[ch32v_rt::interrupt]
fn UART0() {
    // ...
}

#[ch32v_rt::entry]
fn main() -> ! {
    loop {}
}

#[ch32v_rt::highcode]
fn some_highcode_fn() {
    // ...
    // This fn will be loaded into the highcode(SRAM) section.
}
```
