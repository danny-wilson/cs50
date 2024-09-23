# Check for Understanding 5

## Question 1 - Arrays vs. Linked Lists

Recall that, so far, we've seen at least two ways to store a sequence of values: arrays and linked lists.

What's one advantage that using an array has over using a linked list?

|____|

What's one advantage that using a linked list has over using an array?

|____|

## Question 2 - Queues and Stacks

Recall that in lecture, we saw how Jack could use a queue or a stack to organize his clothing. Consider other real-world scenarios where you might want to store physical objects or data using a queue or a stack.

Give an example of a real-world scenario where you might want to store physical objects or data in a stack. Why is a stack the preferred data structure to use for that use case?

|____|

Give an example of a real-world scenario where you might want to store physical objects or data in a queue. Why is a queue the preferred data structure to use for that use case?

|____|

## Question 3 - Deletion

Suppose you're working with a classmate on writing code to remove a linked list from memory. Your classmate suggests writing the following:

```c
free(list);
```

Where `list` is the pointer to the first node in the linked list. Why might this approach *not*, in fact, work well?

|____|

## Question 4 - Memory

Consider the code below:

```c
#include <cs50.h>
#include <stdio.h>
#include <stdlib.h>

int main(void) {

    // Define size of array
    int size = 3;

    // Comment 1
    int *list = malloc(size * sizeof(int));

    // Comment 2
    if (list == NULL) {
        printf("Memory allocation failed\n");
        return 1;
    }

    // Comment 3
    free(list);
}
```

Notice that some of the comments in the code are missing. In the text boxes below, write the comments corresponding to the lines of code above, just like you would do in your own code. Keep in mind that good comments are usually no more than one sentence long.

Comment 1:

[____]()

Comment 2:

[____]()

Comment 3:

[____]()