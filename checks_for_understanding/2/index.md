# Check for Understanding 2

## Question 1 - Command-Line Arguments

Recall that in the lecture, we saw how to write programs in C that support command-line arguments. To do so, we've modified the programs `main` function to take two arguments: `argc` and `agrv`.

### Question 1.1 - Think Back...

What is a program that we have used so far in CS50 that accepts one or more command-line arguments? Name the program, describe what it does (briefly), and describe what the command-line arguments are used for.

|____|

### Question 1.2 - argc and argv

In your own words describe what `argc` is, what it stores and what type it is.

|____|

In your own words describe what `argv` is, what it stores and what type it is.

|____|

## Question 2 - Strings

Consider the two `for` loops, below, both of which print the characters of a string, `s`, one character per line.

```
// Version 1
for (int i = 0; i < strlen(s); i++)
{
    printf("%c\n", s[i]);
}
```

```
// Version 2
for (int i = 0, n = strlen(s); i < n; i++)
{
    printf("%c\n", s[i]);
}
```

In your own words, describe what `strlen` does underneath the hood.

|____|

Which version out of the two is more efficient? Why?

|____|

## Question 3 - More on Strings

Consider the two programs in C below.

**Version 1**
```c
#include <cs50.h>
#include <stdio.h>
#include <string.h>

int main(void) {
    string text = "This is CS50";
    for (int i = 0, length = strlen(text); i < length; i++)
    {
        printf("%c", text[i]);
    }
    printf("\n");
}
```

**Version 2**
```c
#include <cs50.h>
#include <stdio.h>
#include <string.h>

int main(void) {
    string text = "This is CS50";
    for (int i = 0, length = strlen(text); i < length; i++)
    {
        printf("%i", text[i]);
    }
    printf("\n");
}
```

Notice that each program "iterates" over the given variable, `text`, character by character. The output of **Version 1** is, predictably, "This is CS50." But the output of **Version 2** is "84104105115321051153267835348."

In your own words, what is different between the two programs? How does the output of **Version 1** relate to the output of **Version 2**?

|____|