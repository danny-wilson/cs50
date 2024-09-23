# Check for Understanding 6

## Question 1 - Spell Checker

Recall that, in lecture, we saw an implementation of a spell-checker in Python.

Why were we able to implement a spell-checker in Python using fewer lines of code than it took to implement a spell-checker in C?

|____|

Why did the spell checker in Python likely run slower than the spell checker you wrote in C?

|____|

## Question 2 - Compilation vs. Interpretation

Recall from lecture that, whereas C programs are compiled, Python programs are usually interpreted. In your own words, what does it mean for a programming language to be an interpreted language?

|____|

## Question 3 - Loops

Recall that, in C, to get a positive integer between 1 and 8, inclusive, we could use code like the below.

```c
int n;
do
{
    n = get_int("Height: ");
}
while (n < 1 || n > 8);
```

In Python, there are no `do while` loops, so we would express the same idea as the below.


```python
while True:
    n = get_int("Height: ")
    if n >= 1 and n <= 8:
        break
```

Explain how these blocks of code are logically equivalent, as by explaining how each block works line by line.

|____|

## Question 4 - Iteration

Suppose two classmates have written code to iterate over a list of words:

**A**
```py
words = ['Hello', 'world']

for word in words:
    print(word)
```

**B**
```py
words = ['Hello', 'world']

for phrase in words:
    print(phrase)
```

Will the output of these two programs (i.e., what you see on the screen) be any different? Why or why not?

|____|