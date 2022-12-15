#  0x19. C - Stacks, Queues - LIFO, FIFO

## Resources

[Stacks and Queues in C](https://data-flair.training/blogs/stacks-and-queues-in-c/)

## Brief discription

The Monty language

Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). It relies on a unique stack, with specific instructions to manipulate it. The goal of this project is to create an interpreter for Monty ByteCodes files.

## Technology used

gcc 4.8.4

monty 0.98

## Requirements

General

- Allowed editors:`vi`,`vim`, `emacs`
- All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=c89
- All your files should end with a new line
- A README.md file, at the root of the folder of the project is mandatory
- Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
- You allowed to use a maximum of one global variable
- No more than 5 functions per file
- You are allowed to use the C standard library
- The prototypes of all your functions should be included in your header file called monty.h
- Don’t forget to push your header file
- All your header files should be include guarded
- You are expected to do the tasks in the order shown in the project

## Compilation & Output

- Your code will be compiled this way:

       c$ gcc -Wall -Werror -Wextra -pedantic -std=c89 *.c -o monty

- Any output must be printed on stdout
- Any error message must be printed on stderr
   - Here is a link to a GitHub repository that could help you making sure your errors are printed on stderr

## Tasks

Monty Opcodes

- push
  - pushes an element to the stack.

- pall
  - prints all the values on the stack, starting from the top of the stack.

- pint
  - prints the value at the top of the stack,

- pop
  - removes the top element of the stack.

- swap
  - swaps the top two elements of the stack.

- add
  - adds the top two elements of the stack.

- nop
  - does not do anything

- sub
  - subtracts the top element of the stack from the second top element of the stack.

- div
  - divides the second top element of the stack by the top element of the stack.

- mul
  - multiplies the second top element of the stack with the top element of the stack.

- mod
  - computes the rest of the division of the second top element of the stack by the top element of the stack

- pchar
  - prints the char at the top of the stack/queue

- pstr
  - prints the string starting at the top of the stack

- rotl
  - rotates  element at the top to the bottom of the stack

- rotr
  - rotates  element at the bottom to the  top  of the stack

- stack
  - sets the format of the data to a stack (LIFO). Switches a queue to stack mode.v

- queue
  - sets the format of the data to a queue (FIFO).Switches a stack to queue mode.

## Author

Lorrine Adefemi

Sotonye Orifama
