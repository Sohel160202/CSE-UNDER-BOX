# Functions and Program Design

## Objectives

- Divide a program into focused functions.
- Use parameters, return values, and local variables.
- Design a program before writing its implementation.

## Explanation

A function gives a name to a reusable operation. Good functions have one clear responsibility and communicate through parameters and return values.

## Example

    int maximum(int a, int b) {
        return a > b ? a : b;
    }

    int main(void) {
        printf("%d\n", maximum(12, 9));
        return 0;
    }

## Design exercise

Refactor a grade calculator into functions named readMark, calculateGrade, printReport, and isValidMark. Each function should be testable independently.

## Practice

Create a menu application whose actions are implemented by separate functions. Keep main responsible only for program flow.
