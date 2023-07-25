# 0x11. C - printf

## Description
`_printf is a function to do formatted printing output on the screen and it can allow formatting the output in numberous ways. In this printf project we will create a function for simple printing and the format specifications printing.

Depending of the content in the (), this functions use the simple printing or the use or specifiers.

In this project we made the tasks 0 and 1 of mandatory part, and the 14 advanced tasks.

We used a principal function called _printf() for give the string or specifiers to other function called check_format. In this second function search wich specifier is and send it to other funtion that prints the correspondent argument.To understand it easly how it works we prepared flowchart below.
![] (flowchart1.png)
![] (flowchart2.png)
### Conversion specifiers

A character that specifies the type of conversion to be applied. The conversion specifiers and their meaning are:

    d, i: The int argument should be signed decimal notation, and the resulting number is written.
    c: The int argument is converted to a char, and the resulting character is written.
    s: The const char * argument is expected to be a pointer to an array of character type (pointer to a string). Characters from the array are written up to (but not including) a terminating null byte ('\0').
    %: A '%' is written. No argument is converted. The complete conversion specification is '%%'.

## About Functions

### int _putchar(char c)
This function gets a char parameter and writes the parameter to the stdout, the standard output stream.

### int _print_a_char (va_list args)
This function gets a variadic arguments list, traverse the list, prints each character of char type and returns the length of the character.

### int _print_a_string (va_list args)
This function gets a variadic arguments list, traverse the list, prints each string and returns the length of the string.

### int _print_a_integer (va_list args)
This function gets a variadic arguments list, traverse the list, prints each number of int type and returns the length of the integer.

### int _print_format (const char *format, va_list args)
 This function gets a format to be printed and a variadic arguments list, next to check if the format is valid or invalid and according with the verification the resulting output is written to the standard output stream and returns the format length.

### int _print_spec (char format, va_list args):
 This function gets a format valid to be printed and a variadic arguments list to find the format in the list and selects the appropriate function to execute and writes the format to the standard output stream and returns the length of the valid format.

### int _print_invalid_spec (char prev_format, char format, int count)
 This function gets the previous format of the current format, the actual format and the current count of printed characters. Next, the invalid format is written to the standard output stream and returns the length of the invalid format.
 
### void _recursion_integer(int a)
This function gets an integer and prints the last digit of the number as recursion is applied.

### int _validate_char(char _type)
Gets a type and checks if the passed parameter is present in a structure of valid conversion specifiers. Next, returns if the parameter is valid or invalid.

## Return Value
Upon successful return,  _printf() function return the number of characters printed (excluding the null byte used to end output to strings).
If an output error is encountered, a negative value is returned.

Examples

#include "main.h"

_printf("Hello Now"); // the output will be: Hello Now

_printf("%c", 'N'); // the output will be: N

_printf("%s", "Hello Now"); // the output will be: Hello Now

_printf("%!\n"); // the output will be '%!'

_printf("Alx is best: You %s know, Mahari.\n", "should"); // the output will be: Alx is best: You should know, Mahari.

_printf("% s", "Hello"); // the output will be: Hello

_printf("% k"); // the output will be: % k

**Objectives**
- Using git in a team setting
- Applying variadic functions to larger projects
- The complexies of `printf`

---

## Prototype
```C
int _printf(const char *format, ...);
```

### Tasks
### [0. I'm not going anywhere. You can print that wherever you want to. I'm here and I'm a Spur for life](./_printf.c)
* Write a function that produces output according to format
    - c: converts input into a character
    - s: converts input into a string
    - %: prints percentage sign

### [1. Education is when you read the fine print. Experience is what you get if you don't](./printdigit.c)
* Handle the following conversion specifiers
    - d: converts input into a base 10 integer
    - i: converts input into an integer

### and 14 more advanced tasks


### Authors
* **Mahari Tsegay** - [merytseg77@gmail.com](https://github.com/Mahari9)
* **Emmajuliet Awino** - [emmajulietawino14@gmail.com)](https://github.com/AwinoJuliet)
