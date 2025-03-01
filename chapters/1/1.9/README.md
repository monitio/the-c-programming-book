# 1.9 - Character Arrays

Compile with: `gcc src/main.c -o program`

- Only run any of these commands if you have compiled it.
- People who haven't compiled it will have to run the pre-compiled executables to run.
- Run the pre-compiled executables in [the executables folder](./executables/) for your os
Run with: `./program`

[executables](./executables/) | [main.c](./src/main.c)

## important stuff:
- This outline is important to naturally divide the program into pieces:
```c
while (there's another line)
  if (it's longer than the previous longest)
    (save it)
    (save its length)
print (longest line)
```

- `\0` is a null character whose value is `0` (nothing/end)
- `printf` needs and expects `\0` to be at the end of a string

## exercises:
- Exercise 1-16: Revise the main routine of the longest-line program so it will correctly print the length of arbitrary long input lines, and as much as possible of the text.
- Exercise 1-17: Write a program to print all input lines that are longer than 80 characters.
- Exercise 1-18: Write a program to remove trailing blanks and tabs from each line of input, and to delete entirely blank lines.
- Exercise 1-19: Write a function `reverse(s)` that reverses the character string `s`. Use it to write a program that reverses its input a line at a time.
