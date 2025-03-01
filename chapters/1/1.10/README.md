# 1.10 - External Variables and Scope
`getline` has been changed to `mygetline` because of conflicts on POSIX systems.
Do not try and use `getline` thinking it is accessing the books `getline` function.

Compile with: `gcc src/main.c -o program`

- Only run any of these commands if you have compiled it.
- People who haven't compiled it will have to run the pre-compiled executables to run.
- Run the pre-compiled executables in [the executables folder](./executables/) for your os
Run with: `./program`

[executables](./executables/) | [main.c](./src/main.c)

## important stuff:
- variables in `main` such as `line`, `longest`, etc., are private or local to `main` because they are declared in `main` and so no other function can have direct access to them, this is also true for other functions
- local variables only come into existance when the function is called and disappear when the function is exited

- automatic variables are the same as local variables
- automatic variables need to be reset from one call to the next otherwise they will contain garbage

- external variables a.k.a. global variables are accessable by all of the functions (similar to the `#define` tag)
- external variables remain in existance permanently and cannot be deleted
- use `extern` to make an external variable

## exercises:
- Exercise 1-20: Write a program `detab` that replaces tabs in the input with the proper number of blanks to space to the next tab stop. Assume a fixed set of tab stops, say every `n` columns. Should `n` be a variable or a symbolic parameter?
- Exercise 1-21: Write a program `entab` that replaces strings of blanks by the minimum number of tabs and blanks to achieve the same spacing. Use the same tab stops as for `detab`. When either a tab or a single blank would suffice to reach a tab stop, which should be given preference?
- Exercise 1-22: Write a program to `fold` long input lines into two or more shorter lines after the last non-blank character that occurs before the `n`-th column of input. Make sure your program does something intelligent with very long lines, and if there are no blanks or tabs before the specified column.
- Exercise 1-23: Write a program to remove all comments from a C program. Don't forget to handle quoted strings and character constants properly. C comments don't nest.
- Exercise 1-24: Write a program to check a C program for rudimentary syntax errors like unmatched parentheses, brackets and braces. Don't forget about quotes, both single and double, escape sequences, and comments. (This program is hard if you do it in full generality.)
