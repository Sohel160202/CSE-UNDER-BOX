# Structures, Unions, and Data Modeling

## Objectives

- Group related values into structures.
- Access members with dot and arrow operators.
- Explain how a union reuses the same memory area.

## Structure example

    struct Student {
        int id;
        char name[40];
        double cgpa;
    };

    struct Student student = {101, "Asha", 3.75};
    printf("%d %s %.2f\n", student.id, student.name, student.cgpa);

Structures model real entities. They become more useful when combined with arrays, functions, and file-oriented thinking.

A union stores different member types in the same memory location. Only the most recently written member should be treated as valid.

## Practice

Create an array of students. Write functions to add a student, find a student by ID, calculate the class average, and print a report.
