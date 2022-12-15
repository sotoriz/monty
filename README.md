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

### General

- Allowed editors: vi, vim, emacs
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

## More Info

Please use the following data structures for this project. Don’t forget to include them in your header file.

/**
 * struct stack_s - doubly linked list representation of a stack (or queue)
 * @n: integer
 * @prev: points to the previous element of the stack (or queue)
 * @next: points to the next element of the stack (or queue)
 *
 * Description: doubly linked list node structure
 * for stack, queues, LIFO, FIFO
 */
typedef struct stack_s
{
        int n;
        struct stack_s *prev;
        struct stack_s *next;
} stack_t;

/**
 * struct instruction_s - opcode and its function
 * @opcode: the opcode
 * @f: function to handle the opcode
 *
 * Description: opcode and its function
 * for stack, queues, LIFO, FIFO
 */
typedef struct instruction_s
{
        char *opcode;
        void (*f)(stack_t **stack, unsigned int line_number);
} instruction_t;

## Compilation & Output

- Your code will be compiled this way:

$ gcc -Wall -Werror -Wextra -pedantic -std=c89 *.c -o monty

- Any output must be printed on stdout
- Any error message must be printed on stderr
   - Here is a link to a GitHub repository that could help you making sure your errors are printed on stderr

### The monty program

- Usage: monty file
  - where file is the path to the file containing Monty byte code

## Tasks

### Monty Opcodes

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
  - computes the rest of the division of the second top element of the stack/queue by  the top element of the stack

- pchar
  - prints the char at the top of the stack/queue

- pstr
  - prints the string starting at the top of the stack/queue

- rotl
  - rotates  element at the top to the bottom of the stack

- rotr
  - rotates  element at the bottom to the  top  of the stack

- stack
 -sets the format of the data to a stack (LIFO). Switches a queue to stack mode.v

- queue
sets the format of the data to a queue (FIFO).Switches a stack to queue mode.

## Author

Lorrine Adefemi
Sotonye Orifama
