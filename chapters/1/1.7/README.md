# 1.7 - Functions

Compile with: `gcc src/main.c -o program`

- Only run any of these commands if you have compiled it.
- People who haven't compiled it will have to run the pre-compiled executables to run.
- Run the pre-compiled executables in [the executables folder](./executables/) for your os
Run with: `./program`

[executables](./executables/) | [main.c](./src/main.c)

## important stuff:
- Functions have to take on this form:
```c
returnType functionName(parameter declarations, if any) {
  declarations
  statements
}
```

- `return` will decide the output of a function (including main) e.g: `return 0;` for a perfectly fine ending

## exercises:
- Exercise 1-15: Rewrite the temperature conversion program of [Section 1.2](../1.2/) to use a function for conversion.
