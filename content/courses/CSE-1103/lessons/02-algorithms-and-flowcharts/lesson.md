# Algorithms and Flowcharts

## Learning objective

By the end of this lesson, students should be able to describe an algorithm, identify input and output, use sequence, selection, and repetition, and convert a simple algorithm into a flowchart and C program.

## Problem-first example

Create a program that reports whether a number is positive, negative, or zero.

## Algorithm

1. Read a number.
2. If the number is greater than zero, report positive.
3. Otherwise, if the number is less than zero, report negative.
4. Otherwise, report zero.

## Flow structure

Start → Read number → Is number > 0?
- Yes → Positive → End
- No → Is number < 0?
  - Yes → Negative → End
  - No → Zero → End

## C implementation

    #include <stdio.h>

    int main(void) {
        int number;
        scanf("%d", &number);

        if (number > 0) {
            printf("Positive\n");
        } else if (number < 0) {
            printf("Negative\n");
        } else {
            printf("Zero\n");
        }

        return 0;
    }

## Practice

Write algorithms and C programs for:

1. Finding the largest of three numbers.
2. Checking whether a year is a leap year.
3. Calculating a student's grade from marks.
4. Printing all even numbers from 1 to N.

## Challenge

Take one of your algorithms and deliberately introduce an error. Use test inputs to discover the error, explain why it happens, and correct it.

## Assessment

Submit:

- The problem statement
- The algorithm
- The flowchart
- The C program
- Three test cases
- A short explanation of your debugging process
