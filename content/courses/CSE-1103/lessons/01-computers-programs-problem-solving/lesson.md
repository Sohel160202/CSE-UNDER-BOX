# Computers, Programs, and Problem Solving

## Learning objective

By the end of this lesson, students should be able to explain how a problem becomes a running program and identify the roles of hardware, software, source code, compiler, executable, and runtime input.

## Start with a problem

A student wants to calculate the average marks of three subjects. Before writing code, we need to identify:

- What information enters the system?
- What calculation is required?
- What result should be produced?
- What rules should the program follow?

## Concept map

Problem → Analysis → Algorithm → Source Code → Compilation → Testing → Result

## Core explanation

A computer does not understand an informal problem statement directly. A programmer converts the problem into a precise sequence of operations. That sequence is the algorithm. A programming language expresses the algorithm in a form that can be compiled or interpreted.

For this course, C will be the first implementation language because it makes program structure, memory, types, and control flow visible.

## Worked example

Problem: calculate the average of three integers.

Algorithm:

1. Read three marks.
2. Add the marks.
3. Divide the sum by three.
4. Display the average.

C implementation:

    #include <stdio.h>

    int main(void) {
        int first, second, third;

        scanf("%d %d %d", &first, &second, &third);

        double average = (first + second + third) / 3.0;
        printf("Average: %.2f\n", average);

        return 0;
    }

## Think and try

Change the program so it also prints:

- The total marks
- The highest mark
- Whether the student passed

## Common mistakes

- Dividing by 3 when an integer average is not intended.
- Forgetting the address operator in scanf.
- Not checking whether the input follows the expected format.
- Treating source code and the executable file as the same thing.

## Assessment

Explain, in your own words, the difference between an algorithm, source code, a compiler, and an executable program.

## Further resources

External videos and university lectures will be added after review and mapped to the exact concepts in this lesson.
