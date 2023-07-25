# 0x11. C - printf

## Description
`_printf is a function to do formatted printing output on the screen and it can allow formatting the output in numberous ways. In this printf project we will create a function for simple printing and the format specifications printing.

Depending of the content in the (), this functions use the simple printing or the use or specifiers.

In this project we made the tasks 0 and 1 of mandatory part, and the 14 advanced tasks.

We used a principal function called _printf() for give the string or specifiers to other function called check_format. In this second function search wich specifier is and send it to other funtion that prints the correspondent argument.To understand it easly how it works we prepared flowchart below.

![](_printf function flowchart.drawio.png)
![](function check format.png)

### Conversion specifiers

A character that specifies the type of conversion to be applied. The conversion specifiers and their meaning are:

    d, i: The int argument should be signed decimal notation, and the resulting number is written.
    c: The int argument is converted to a char, and the resulting character is written.
    s: The const char * argument is expected to be a pointer to an array of character type (pointer to a string). Characters from the array are written up to (but not including) a terminating null byte ('\0').
    %: A '%' is written. No argument is converted. The complete conversion specification is '%%'.


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
