# 0x19. C - Stacks, Queues - LIFO, FIFO

## Description

This project is a custom ByteCode interpreter, coded in C.
Compilation:
```gcc -Wall -Werror -Wextra -pedantic *.c
-o monty```
Usage:
```./monty byte_file.m```

The monty program

Usage: monty file
where file is the path to the file containing Monty byte code
If the user does not give any file or more than one argument to your program, print the error message USAGE: monty file, followed by a new line, and exit with the status EXIT_FAILURE
If, for any reason, it’s not possible to open the file, print the error message Error: Can't open file <file>, followed by a new line, and exit with the status EXIT_FAILURE
where <file> is the name of the file
If the file contains an invalid instruction, print the error message L<line_number>: unknown instruction <opcode>, followed by a new line, and exit with the status EXIT_FAILURE
where is the line number where the instruction appears.
Line numbers always start at 1
The monty program runs the bytecodes line by line and stop if either:
it executed properly every line of the file
it finds an error in the file
an error occured
If you can’t malloc anymore, print the error message Error: malloc failed, followed by a new line, and exit with status EXIT_FAILURE.
You have to use malloc and free and are not allowed to use any other function from man malloc (realloc, calloc, …)

## Table of contents

File | Description
---- | -----------
[main.c](./main.c) | entry point of the program
[monty.h](./monty.h) | main header file
[lists.h](./lists.h) | header file for the lists functions
[get_func.c](./get_func.c) | function that picks the right function for the instruction
[handler_funcs1.c](./handler_funcs1.c) | handler functions for the instructions
[handler_funcs2.c](./handler_funcs2.c) | handler functions for the instructions
[handler_funcs3.c](./handler_funcs3.c) | handler functions for the instructions
[list_funcs1.c](./list_funcs1.c) | doubly linked list functions
[list_funcs2.c](./list_funcs2.c) | doubly linked list functions
[strtow.c](./strtow.c) | string tokenizing functions
[free.c](./free.c) | memory handling functions
[char.c](./char.c) | handler functions for ascii instructions
[bf](./bf) | Advanced tasks: Brainf*ck programs
