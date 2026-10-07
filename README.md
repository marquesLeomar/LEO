# 🦁 LEO (Lion) Programming Language

![Status](https://img.shields.io/badge/Status-In%20Development-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

**LEO** is a modern programming language designed to be simpler and cleaner than Python, yet built from day one to tackle hardware challenges and the future of computing. The lion roars where other languages run out of breath.

## 🎯 The Vision

LEO was born to unify ecosystems that historically demand entirely different toolchains. Our goal is to let you write clean, declarative code that can run on a low-cost microcontroller, train a neural network, or manipulate quantum states—all with the exact same simplicity.

## 🚀 Key Features

- **Extreme Simplicity:** No unnecessary curly braces `{}`, no semicolons `;`. It uses inferred static typing that prevents errors without cluttering your code.
- **Embedded First (IoT & Hardware):** Native (Zero Overhead) transpilation to C/C++. Perfect for ESP32, STM32, and bare-metal/FreeRTOS architectures. GPIO control and hardware interrupts are treated as first-class citizens.
- **AI & Data Analysis:** Native structures for matrices and tensors. Seamless integration with vector processing and Machine Learning routines, simplifying computer vision and prediction pipelines.
- **Quantum-Ready:** Built-in abstractions for Qubits and quantum logic gates, designed to integrate smoothly with quantum circuit compilers (like OpenQASM).
- **Highly Documented:** Born to be clear. LEO prioritizes human-readable error messages and documentation tailored for rapid adoption by engineers and scientists.

## 💻 What does it look like? (Concept)

*A glimpse of how LEO approaches a classic embedded problem (Blink) with clean syntax:*

```leo
# LEO is clean and straightforward
config pin_led = 2
config delay_time = 500 ms

routine smart_blink():
    while true:
        turn_on(pin_led)
        wait(delay_time)
        turn_off(pin_led)
        wait(delay_time)
