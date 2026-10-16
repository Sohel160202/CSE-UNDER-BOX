# Decision Making

## Objectives

- Use if, else if, else, and switch.
- Design mutually exclusive and independent conditions.
- Test boundary values.

## Explanation

A decision lets a program choose a path. Conditions should be written so every valid input has a defined outcome.

Use if statements for ranges and compound conditions. Use switch when one expression is compared against several constant cases.

## Example

    if (mark >= 80) {
        grade = 'A';
    } else if (mark >= 70) {
        grade = 'B';
    } else if (mark >= 60) {
        grade = 'C';
    } else {
        grade = 'F';
    }

## Debugging activity

Test exactly 80, 79, 70, 69, 60, 59, and invalid marks. Explain what each test proves.

## Practice

Create a menu-driven unit converter using switch. Support kilometres/miles, Celsius/Fahrenheit, and kilograms/pounds.
