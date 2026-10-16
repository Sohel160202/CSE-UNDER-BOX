# Arrays and Strings

## Objectives

- Store and process collections of values.
- Traverse arrays safely.
- Use C strings and understand the terminating null character.

## Explanation

An array stores elements of the same type in contiguous memory. Indexing starts at zero. A C string is an array of char values ending with the null character.

## Example

    int marks[5] = {72, 81, 64, 90, 77};
    int total = 0;

    for (int i = 0; i < 5; i++) {
        total += marks[i];
    }

    printf("Average: %.2f\n", total / 5.0);

## Safety checklist

- Never read beyond the final valid index.
- Reserve space for the string terminator.
- Define the maximum input length.
- Test empty and maximum-length input.

## Practice

Find the minimum, maximum, average, and second-highest mark in an array. Then count vowels and words in a sentence.
