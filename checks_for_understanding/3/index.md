# Check for Understanding 3

## Question 1 - Structs

Recall from lecture how we implemented a phone book in C using the below `struct`.

```c
typedef struct
{
    string name;
    string number;
}
person;
```

Why was it arguably better design to use one array of `struct`s than to use two arrays, one to store names and one to store phone numbers?

|____|

Imagine you were to use the above `struct` to implement an app for your contacts, like the one on your mobile phone. What are two additional fields might you want to add to the `struct`, what should their types be, and why?

|____|


## Question 2 - Searching and Sorting

Imagine that you have an unsorted collection of items (maybe they're notes for class or a collection of old receipts) that you expect you'll need to search.

Under what circumstances might it make more sense to sort the collection of items first before searching, and under what circumstances might it make more sense to leave the collection unsorted?

*Hint: Consider algorithmic efficiency. What's the cost (i.e., running time) of linear search? Of binary search? Of sorting?*

|____|

## Question 3 - Recursion 

Consider the code below that calculated the factorial of a provided number using recursion. 

```c
#include <cs50.h>
#include <stdio.h>

// Prototype for factorial function
int factorial(int n);

int main()
{
    int number;
    
    // Prompt user for a number
    do
    {
        number = get_int("Please input a number: ");
    }
    // Comment 1
    while (number < 0);

    int result = factorial(number);
    printf("The factorial of %i is %i\n", number, result);
}

// Comment 2
int factorial(int n)
{
    // Comment 3
    if (n == 0) 
    {
        return 1;
    }

    // Comment 4
    return n * factorial(n - 1);
}
```

### Question 3.1 - Comments

As you might have noticed, some comments in the program are missing! In the following answer boxes, provide comments for each of the corresponding lines.

Comment 1: *Why the number can't be negative?*

[____]()

Comment 2: *What does the `factorial` function do?*

[____]()

The next two comments are related to two key components of any recursion algorithm. 

Comment 3: *What does this block of code represent?*

[____]()

Comment 4: *How does this block of code compute a factorial?*

[____]()

### Question 3.2 - Back to the basics

Now, in your own words, describe what recursion is. In particular, describe the key components of recursion. Why are they important?

|____|