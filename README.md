# Ishan Bijukuchhay

Computer Engineering @ Queen's University. Firmware and embedded systems.

## About

I work close to the hardware — bare-metal C, register-level programming,
and systems where you can measure what you built and explain why it
behaves the way it does. Most of what I put here is built from datasheets
and reference manuals rather than libraries, because the point is to
understand the layer underneath.

## Projects

**[stm32-drivers](https://github.com/ishjuke/stm32-drivers)** — Bare-metal
driver stack for the STM32F401RE (Cortex-M4) in C. No HAL, no generated
code: custom linker script, vector table, C runtime startup, register-level
GPIO, and an interrupt-driven UART with a ring buffer. Verified with GDB,
disassembly of the flashed binary, and a logic analyzer — proving each
peripheral works rather than assuming it from the output.

**[caching-proxy](https://github.com/ishjuke/caching-proxy)** — HTTP caching
reverse proxy in C on a Raspberry Pi 5. Four concurrency models
(single-threaded, thread-per-connection, thread pool, epoll) benchmarked
against each other over wired Ethernet with nginx as origin. ~29× throughput
on cache hits; LRU held 75% hit rate against LFU's 9.5% under drifting load.

## Currently

Extending the STM32 stack with an I2C sensor driver, and working through
DSA in C.

## Elsewhere

[Portfolio](https://ishanbijukuchhay.com) ·
[LinkedIn](https://www.linkedin.com/in/ishan-bijukuchhay/) ·
ishanbijukuchhay@gmail.com
