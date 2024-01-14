# holbertonschool-monty
# C - Stacks, Queues - LIFO, FIFO

## Monty 0.98 Interpreter
This is an interpreter for Monty ByteCode files, written in C. Monty is a scripting language that is first compiled into Monty byte codes and relies on a unique stack, with specific instructions to manipulate it.

## Requirements
The interpreter follows the following requirements:

* If the user does not give any file or more than one argument to the program, it will print the error message "USAGE: monty file", followed by a new line, and exit with the status EXIT_FAILURE.

* If, for any reason, it’s not possible to open the file, the interpreter will print the error message "Error: Can't open file ", followed by a new line, and exit with the status EXIT_FAILURE, where is the name of the file.

* If the file contains an invalid instruction, the interpreter will print the error message "L<line_number>: unknown instruction", followed by a new line, and exit with the status EXIT_FAILURE, where <line_number> is the line number where the instruction appears.

* Line numbers always start at 1.

* The interpreter runs the bytecodes line by line and stops if either:

** It executed properly every line of the file.
** It finds an error in the file.
** An error occurred.
* If the interpreter can’t malloc anymore, it will print the error message "Error: malloc failed", followed by a new line, and exit with status EXIT_FAILURE.

The interpreter uses malloc and free and is not allowed to use any other function from man malloc (realloc, calloc, …).

## Usage
To use the interpreter, run the following command:
```
$ ./monty <file>
```
Where is the path to the file containing Monty byte code.

## File Description
The project includes the following files:

1. functions.c: contains functions:
* push: pushes an element to the stack.
* pall: prints ALL values on the stack, starting from the top of the stack.
* pint: prints SPECIFICALLY the value at the top of the stack, followed by a newline.
* pop: removes SPECIFICALLY the top element of the stack.
* free_stack: frees memory allocated to all nodes in a linked stack.
2. more_functions.c: contains functions:
* swap: swaps SPECIFICALLY the top two elements of the stack.
* add: adds SPECIFICALLY the top two elements of the stack.
* nop: does nothing.
3. monty.h: contains structures and function initialization.
4. main.c: contains functions:
* main: monty code interpreter.
5. fstruct.c: contains functions:
* read_lines: reads each line of a file.
* interpret_line - interprets a single line of the file.
* monty_interpreter - Interpreter for themonty functions.


## Authors
![GitHub Contributors Image](https://contrib.rocks/image?repo=anacardona0220/holbertonschool-higher_level_programming) Ana Maria Cardona Botero - <a href="https://github.com/anacardona0220" target="_blank"> @anacardona0220</a> :genie_woman:![Your Repository's Stats](https://github-readme-stats.vercel.app/api?username=anacardona0220&show_icons=true)

