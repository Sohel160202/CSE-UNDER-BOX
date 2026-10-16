# Data Types, Input, Output, and Expressions

## Objectives

- Use identifiers, variables, constants, and primitive data types.
- Read values with scanf and display formatted output with printf.
- Evaluate arithmetic, relational, and logical expressions.

## Core ideas

A variable is a named storage location. Its type determines what values it can represent and how the compiler interprets its memory. Common types include int, float, double, char, and void.

Operators form expressions. Arithmetic operators calculate values, relational operators compare values, and logical operators combine conditions.

## Example

    int quantity;
    double price;

    scanf("%d %lf", &quantity, &price);
    double total = quantity * price;
    printf("Total: %.2f\n", total);

## Common mistakes

- Using the wrong conversion specifier.
- Forgetting the address operator during input.
- Assuming integer division produces a fractional result.
- Naming variables with spaces or reserved keywords.

## Practice

Build a simple electricity-bill calculator. Read units consumed and price per unit, then print the subtotal, tax, and final bill.
