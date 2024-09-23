# Check for Understanding 4

## Question 1 - Enhance

Take a look at [this video](https://www.youtube.com/watch?v=i3gv2zOmJiA), which shows an image being "enhanced" to reveal additional details in the reflection of a person's sunglasses. Why is that process likely unrealistic?

|____|

## Question 2 - Square

Recall that, in lecture, we saw how every time we call a function in C, some memory is allocated on the stack to store that function's variables. Consider the following C program, which attempts to take a number and print out its square.

```
#include <stdio.h>

void square(int x);

int main(void)
{
    int x = 5;
    square(x);
    printf("%i\n", x);
}

void square(int n)
{
    n = n * n;
}

```

But when compiled and run, this program prints out the number 5, instead of 25 (the square of 5).

Why does the program not print 25? What change(s) could we make to this program to fix the bug?

|____|

## Question 3 - Pointers

Consider these statements below.

```c
int x = 4;
int *p1 = &x;
int *p2 = p1;
*p2 = 3;
```

If you were to print out the above variables, what would be the printed values of `x`, `*p1`, and `*p2`? Try using pencil and paper to reason your way through, and explain why the values are identical or different.

|____|

## Question 4 - Hexadecimals and Colors

Recall from lecture that hexadecimal is a base-16 counting system That is, hexadecimal uses 16 distinct symbols to represent numbers:

```text
0 1 2 3 4 5 6 7 8 9 A B C D E F
```

For example, the decimal number `12` is `C` in hexadecimal. And the decimal number `221` is `DD` in hexadecimal.

Recall that one way computers represent color is by the color's relative concentration of red, green, and blue (RGB!).

Using [this website](https://htmlcolorcodes.com/), try the following:

* Using the slider and clicker, choose a color that you like.
* Notice the RGB values associated with that color.
* Notice the hex value associated with that color.

In general, what is the relationship between RGB and hexadecimal values associated with the same color?

|____|