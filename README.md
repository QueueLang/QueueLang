# QueueLang

QueueLang is a versatile interpreted programming language written in C++. Designed for simplicity and speed, it features a queue-inspired syntax while supporting advanced constructs like functions and lambdas. Whether you're building simple scripts or complex applications, QueueLang provides a powerful and efficient way to write code.

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

console.out(x + y)
```
## Functions And Lambdas

You can define functions and use lambdas in QueueLang to create more dynamic and reusable code:

### Function Example:
```queue
func add(x, y) {
    return x + y
}

console.out(add(6 + 3))
```

### Lambda Example:
```queue
add = lambda x, y: x + y

console.out(add(4 + 12))

```
---
## Download and Usage

### Download QueueLang

[Download the latest version of QueueLang here](https://github.com/QueueLang/QueueLang/releases)

### Run/Compile QueueLang

To run a QueueLang file (.ql), execute this command in terminal:
```queue
queuelang your-file.ql
```

To compile a QueueLang file, execute this command instead:
```queue
queuelang -compile your-file.ql -o your-file.exe
```
When compiling, you can choose either a .exe file (given in the example command above), or create it without an extension. On Windows, both are valid methods of compiling. Although on Mac/Linux, you are required to use the one without the extension. Either way, to execute it, just run:
```queue
./your-file
```

---

## Documentation

For more detailed documentation, please refer to the [QueueLang Wiki](https://github.com/QueueLang/QueueLang/wiki).

---

## Contributing

We welcome contributions! To get started, fork the repository, create a new branch, and submit a pull request. You can also contribute by joining the organization to help develop this project! [Visit The QueueLang Community](https://github.com/Quemunnity)

---

## License

QueueLang is open source and released under the [MIT License](https://raw.githubusercontent.com/QueueLang/QueueLang/refs/heads/main/LICENSE).

---

***© 2024 QueueLang Project. All rights reserved.***
