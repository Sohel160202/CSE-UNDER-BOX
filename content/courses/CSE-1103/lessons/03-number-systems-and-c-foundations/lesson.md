# Number Systems and C Foundations

## Objectives

- Convert between binary, decimal, and hexadecimal.
- Explain how characters are represented by codes.
- Describe the purpose of a compiler and the basic structure of a C program.

## Concepts

Computers store information as bits. A group of eight bits is a byte. Decimal is convenient for people, while binary reflects digital hardware and hexadecimal provides a compact representation of binary values.

C programs are text files that are translated by a compiler into an executable program. A minimal program has an entry point called main.

## Example

    #include <stdio.h>

    int main(void) {
        printf("Hello, CSE Under Box!\n");
        return 0;
    }

The preprocessor includes the standard input/output declarations. The main function is where execution begins. Returning zero communicates successful completion.

## Practice

Convert 45 from decimal to binary and hexadecimal. Then write a program that prints your name, department, and three learning goals.
