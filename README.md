<a href="https://www.cprogramming.com"><img src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white" height="25em" alt="C"/></a>

# Ft_Printf

## Goal

Recreate a simplified version of the printf function from the C standard library. The function should handle various format specifiers (e.g., %d, %s, %x) and output formatted strings to the standard output.

## Key Features

- Format Specifiers: Supports common specifiers like %c, %s, %d, %i, %u, %x, %X, %p, and %%.
- Variable Arguments: Uses va_list and va_arg to handle a variable number of arguments.
- Output: Writes the formatted string to standard output.
- Custom Implementation: Reimplements core functionality without relying on the standard printf.

## Implementation Details

- Parsing: Parses the format string to identify specifiers and their corresponding arguments.
- Conversion: Converts arguments to their appropriate string representation (e.g., numbers to strings, pointers to hexadecimal addresses).
- Output Management: Writes the formatted string to the standard output using write.
- Edge Cases: Handles edge cases like null strings, invalid specifiers, and zero values.

## Challenges

- Specifiers: Implementing each specifier correctly and efficiently.
- Memory Management: Ensuring there are no memory leaks, especially when handling dynamic conversions.
E- dge Cases: Handling unusual inputs like empty strings, null pointers, or mixed format specifiers.

## Skills Developed

- Variadic Functions: Learning to use va_list, va_arg, and va_start to handle variable arguments.
- String Manipulation: Implementing conversions for different data types to strings.
- Edge Case Handling: Testing and debugging to ensure robustness.

## Installation

1. Clone the repository:
```sh
git clone git@github.com:casomarr/42-Ft_Print.git
```
2. Add a main function at the end of the ft_printf.c file to test the ft_print function:
```c
#include "ft_printf.h"  

int main(void) {  
    ft_printf("Hello, %s! The number is %d.\n", "World", 42);  
    ft_printf("Pointer: %p\n", "Test");  
    ft_printf("Hexadecimal: %x\n", 255);  
    ft_printf("Unsigned: %u\n", -42);  
    return (0);  
}
```
3. Compile the program:
```sh
make 
```
4. Run the program to test its functionality:
```sh
./ft_printf
``` 
