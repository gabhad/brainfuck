# Brainfuck Interpreter in C++

This repository contains a simple Brainfuck interpreter written in C++. The interpreter reads and executes Brainfuck code from a given file.

## Prerequisites

- Make sure you have a C++ compiler installed (like `g++`).

## Building the Interpreter

To build the Brainfuck interpreter, simply navigate to the repository directory and run `make`:

```sh
make
```

## Running the Interpreter

To run the Brainfuck interpreter, use the mindopen executable followed by the path to a file containing Brainfuck code:

```sh
./mindopen path/to/brainfuck/code/file.bf
```

Replace `path/to/brainfuck/code/file.bf` with the actual path to your Brainfuck code file.

## Example

If you have a Brainfuck code file named hello.bf, you can run the interpreter like this:

```sh
./mindopen hello.bf
```

## Brainfuck Language Overview
Brainfuck is a minimalistic esoteric programming language with only eight commands, each represented by a single character:

- `>`: Increment the data pointer.
- `<`: Decrement the data pointer.
- `+`: Increment the byte at the data pointer.
- `-`: Decrement the byte at the data pointer.
- `.`: Output the byte at the data pointer.
- `,`: Accept one byte of input, storing its value in the byte at the data pointer.
- `[`: If the byte at the data pointer is zero, jump forward to the command after the matching ].
- `]`: If the byte at the data pointer is nonzero, jump back to the command after the matching [.

Brainfuck operates on an array of memory cells, each initially set to zero. The data pointer starts at the beginning of this array. The language is Turing complete, meaning it can theoretically solve any computation problem given enough time and memory.

For more details on the Brainfuck language, refer to the [Wikipedia](https://en.wikipedia.org/wiki/Brainfuck) page.

## Test Files
Some example Brainfuck programs are provided in the `test/` directory. You can use these files to test the interpreter. To run a test file, use the following command:

```sh
./mindopen test/filename.bf
```
Replace `filename.bf` with the name of the test file you want to execute.

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.
