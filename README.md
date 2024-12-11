# QueueLang

QueueLang is a versatile interpreted programming language written in C++. Designed for simplicity and speed, it features a queue-inspired syntax while supporting advanced constructs like functions and lambdas. Whether you're building simple scripts or complex applications, QueueLang provides a powerful and efficient way to write code.

---

## Features

- **Interpreted Language**: Quickly test and run your code without the need for complex compilation steps.
- **Queue-Inspired Syntax**: A unique queue-based structure for variable declaration and operations.
- **Functions and Lambdas**: Support for defining functions and using lambda expressions.
- **Written in C++**: High-performance implementation with low overhead.
- **Simple and Powerful**: Combines simplicity of Python with advanced features for more complex applications.
- **Plugin System**: Easily integrate Python-based plugins using the `.qlpkg` file format, and handle circular dependencies with the `.dependencies` file.

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
---

## Functions And Lambdas

You can define functions and use lambdas in QueueLang to create more dynamic and reusable code:

### Function Example:
```queue
func add(x, y) {  
    return x + y  
}

console.out(add(6 + 3))

### Lambda Example:
add = lambda x, y: x + y

console.out(add(4 + 12))
```

---

## Plugin System

QueueLang supports integrating Python-based plugins through the `.qlpkg` file format. The plugins are automatically included and interpreted during runtime.

### How It Works

- When importing plugins in your `.ql` file, QueueLang checks the `.dependencies` file to see if the required `.qlpkg` file has been included before.
- If the plugin is not already included, QueueLang appends the `.qlpkg` content to the current `.ql` file, ensuring no duplicates and avoiding circular dependencies.
- The `.dependencies` file is used to track which plugins have already been added, with each plugin name stored without the extension. For example:

```dependencies
your_plugin  
math  
system  
os
```

---

## Download and Usage

### Download QueueLang

[Download the latest version of QueueLang here](https://github.com/QueueLang/QueueLang/releases)

### Run/Compile QueueLang

**Remember that in these examples, you don't have to use 'your-file' or 'your-package'. You may use any name you wish.**

To run a QueueLang file (.ql), execute this command in terminal:  
`queuelang your-file.ql`

To compile a QueueLang file, execute this command instead:  
`queuelang -compile your-file.ql -o your-file.exe`

When compiling, you can choose either a .exe file (given in the example command above), or create it without an extension. On Windows, both are valid methods of compiling. Although on Mac/Linux, you are **REQUIRED** to **omit the .exe extension**. Either way, to execute it, just run:  
`./your-file`

To compile a QueueLang package, execute:  
`queuelang -compilepkg your-package.py -o your-package.qlpkg`

The `-o` flag is not required, but if omitted, the output file will default to `queuelang_package.qlpkg`. The `-o` flag allows you to customize the output file name. You **CANNOT** change the extension (.qlpkg) to something different. If you do, it will result in a plugin parser error. Python plugin files (.py) will compile into the `.qlpkg` file and be used during runtime evaluations and within the QueueLang scripts themselves.

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
