
# C - Sorting algorithms & Big O

## Resources

*Read or watch:*

- [Sorting algorithm](https://intranet.alxswe.com/rltoken/-j5MKLBlzZAC2RfJ5DTBIg)
- [Big O notation](https://intranet.alxswe.com/rltoken/WRvrE2BaNVQFssHiUATTrw)
- [Sorting algorithms animations](https://intranet.alxswe.com/rltoken/ol0P7NbYVb5R31iOv4Q40A)
- [15 sorting algorithms in 6 minutes](https://intranet.alxswe.com/rltoken/_I0aEvhfJ66Xyob6dd9Utw) (WARNING: The following video can trigger seizure/epilepsy. It is not required for the project, as it is only a funny visualization of different sorting algorithms)
- [CS50 Algorithms explanation in detail by David Malan](https://intranet.alxswe.com/rltoken/Ea93HeEYuNkOL7sGb6zzGg)
- [All about sorting algorithms](https://intranet.alxswe.com/rltoken/21X_eaj5RGcLIL9mZv2sqw)

## General

- At least four different sorting algorithms
- What is the Big O notation, and how to evaluate the time complexity of an algorithm
- How to select the best sorting algorithm for a given input
- What is a stable sorting algorithm

## More Info

### Data Structure and Functions

- For this project you are given the following print_array, and print_list functions:

```
#include <stdlib.h>
#include <stdio.h>

/**
 * print_array - Prints an array of integers
 *
 * @array: The array to be printed
 * @size: Number of elements in @array
 */
void print_array(const int *array, size_t size)
{
    size_t i;

    i = 0;
    while (array && i < size)
    {
        if (i > 0)
            printf(", ");
        printf("%d", array[i]);
        ++i;
    }
    printf("\n");
}
```

```
#include <stdio.h>
#include "sort.h"

/**
 * print_list - Prints a list of integers
 *
 * @list: The list to be printed
 */
void print_list(const listint_t *list)
{
    int i;

    i = 0;
    while (list)
    {
        if (i > 0)
            printf(", ");
        printf("%d", list->n);
        ++i;
        list = list->next;
    }
    printf("\n");
}
```
