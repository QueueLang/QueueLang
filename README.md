# QueueLang

QueueLang is a versatile interpreted programming language written in C++. Designed for simplicity and speed, it features a queue-inspired syntax while supporting advanced constructs like functions and lambdas. Whether you're building simple scripts or more complex applications, QueueLang provides a powerful and efficient way to write code.

---

## Features

- **Interpreted Language**: Quickly test and run your code without the need for complex compilation steps.
- **Queue-Inspired Syntax**: A unique queue-based structure for variable declaration and operations.
- **Functions and Lambdas**: Support for defining functions and using lambda expressions.
- **Written in C++**: High-performance implementation with low overhead.
- **Simple and Powerful**: Combines simplicity of Python with advanced features for more complex applications.

---

## Installation

To get started with QueueLang, simply download the latest release from the [releases page](https://github.com/QueueLang/QueueLang/releases).

### Requirements

- C++ compiler (for building the language)
- Python (for running plugins)
  
---

## Basic Syntax

QueueLang uses a simple queue-like syntax for defining variables and performing operations. Here's an example of basic usage:

```queue
queue x = 0
queue y = 5

console.out(toString(x + y))
