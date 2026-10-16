# Pointers, Memory, and Scope

## Objectives

- Explain addresses, values, and pointers.
- Use pointers for controlled data access and output parameters.
- Distinguish local, global, and parameter scope.

## Explanation

A pointer stores the address of another object. The address operator obtains an address, and the dereference operator accesses the value at that address.

    void swap(int *a, int *b) {
        int temp = *a;
        *a = *b;
        *b = temp;
    }

Pointers are powerful because they allow functions to modify caller-owned data. They are dangerous when they point to invalid memory.

## Rules

- Initialize pointers before use.
- Never dereference a null or uninitialized pointer.
- Keep ownership and lifetime clear.
- Prefer small, testable functions.

## Practice

Implement swap, minimum-and-maximum output parameters, and a function that reverses an array using pointer arithmetic.
