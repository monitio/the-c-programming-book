# 1.5 - Character Input and Output
I have combined all sub-categories into just one category.
1.5 itself doesn't have any important code so i have just removed it.

Compile 1.5.1 with: `gcc src/1-5-1.c -o 1-5-1`
Compile 1.5.1.2 with: `gcc src/1-5-1.2.c -o 1-5-1-2`
Compile 1.5.2 with: `gcc src/1-5-2.c -o 1-5-2`
Compile 1.5.2.2 with: `gcc src/1-5-2.2.c -o 1-5-2-2`
Compile 1.5.3 with: `gcc src/1-5-3.c -o 1-5-3`
Compile 1.5.4 with: `gcc src/1-5-4.c -o 1-5-4`

- Only run any of these commands if you have compiled it.
- People who haven't compiled it will have to run the pre-compiled executables to run.
- Run the pre-compiled executables in [the executables folder](./executables/) for your os
Run 1.5.1 with: `./1-5-1`
Run 1.5.1.2 with: `./1-5-1.2`
Run 1.5.2 with: `./1-5-2`
Run 1.5.2.2 with: `./1-5-2.2`
Run 1.5.3 with: `./1-5-3`
Run 1.5.4 with: `./1-5-4`

[executables](./executables/) | [all code](./src/)

## important stuff:
- a text stream is a sequence of characters divided into lines; each line consists of zero or more characters followed by a newline character

- the C standard library provides several functions for reading or writing one character at a time of which `getchar()` and `putchar()` are the simplest
- `getchar()` reads the next input character from a text stream and returns that as its value after: `c = getchar();` gets called.
- the variable `c` contains the next character of input that normally comes from the keyboard
- the function `putchar()` prints a character each time it is called.
- `putchar(c);` prints the contents of the integer variable `c` as a character, usually shown on screen
- calls to `putchar()` and `getchar()` may be interleaved
- the output will appear in the order in which the calls are made

### 1.5.1:
- `!=` means "not equal to"
- `EOF` means "end of file" and is an integer

- `getchar()` returns a value when there is no more input
- `c = getchar();` is an expression and therefore has a value
- less calls of `getchar()` means smaller executable size

- `c = getchar() != EOF` is equivalent to `c = (getchar() != EOF)`

#### exercises:
- Exercise 1-6: Verify that the expression `getchar() != EOF` is 0 or 1.
- Exercise 1-7: Write a program to print the value of `EOF`.

### 1.5.2:
- `++` means to increment by one and is more consise and efficient than just adding one normally
- `--` is the opposite to `++` and decrements by one

- `++` is equivalent to `a = a + 1` (example different to book)
- `--` is equivalent to `a = a - 1` (example different to book)

- `--` or `++` can be either prefixes or suffixes (book calls them either prefix and postfix operators)

- to cope with bigger numbers use a `double` (double precision `float`)

#### exercises:
None listed in book.

### 1.5.3:
- `A` is 65 in the ASCII character set
- `\n` or a newline character is 10 in the ASCII character set (see [chapter 2](../../) (not done yet) for strings vs characters)
- `\n` counts as a newline character or one character not 2, not more just one character (see [chapter 2](../../) (not done yet) for strings vs characters)

- `==` is the C notation for "is equal to" and triggers an equality test

- a character written between single quotes represents an integer value equal to a machines numerical character value in the machines character set

#### exercises:
- Exercise 1-8: Write a program to count blanks, tabs, and newlines.
- Exercise 1-9: Write a program to copy its input to its output, replacing each string of one or more blanks by a single blank.
- Exercise 1-10: Write a program to copy its input to its output, replacing each tab by `\t`, each backspace by `\b`, and each backslash by `\\`. This makes tabs and backspaces visible in an unambiguous way.

### 1.5.4:
- `||` means "OR"
- `&&` means "AND"
- `&&` and `||` both go left to right

- `nl = nw = nc = 0;` sets all three variables to zero

#### exercises:
- Exercise 1-11: How would you test the word count program? What kinds of input are most likely to uncover bugs if there are any?
- Exercise 1-12: Write a program that prints its input one word per line.
