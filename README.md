
# prinf function using C programming

The printf function sends the formatted output to stdout. We replicating the the printf function with our custom _printf(). The purpose is to teach us how to develop _printf()._printf() function format string is a character string, beginning and ending in its initial shift state, if any. These arguments are placed using the percentage '%' operator
##

#### Resources
Secrets of printfby Don colton https://www.cypress.com/file/54761/download
##
#### Compilation and installation
The code must be checked with betty: 
####


````bash
*$ betty _printf.c
````

The code must be compiled this way:
````bash
 *$ gcc -Wall -Werror -Wextra -pedantic.c
 ````

 As a consequence, be careful not to push any c file containing a main function in the root directory of your project (you could have a test folder containing all your tests files including main functions)

The main files will include your main header file (main.h): #include main.h
 ##
#### Use & Examples
Prototype: int _printf(const char *format, ...); Use - General: _printf("format string", var1, var2, ...);

Examples:

- Basic String: _printf("%s Julian", "Hello");`

    - Output: Hello Julian

- Print integers: _printf("This is an array element: arr[%d]:%c", 32, arr[32]);`

    - Output: This is an array element arr[32]:A
Many other specifiers and flags were added and by combinig those the _printf() function generate a different ouput. The following list are the specifiers and flags allowed.
##

Use & Examples

#### Specifiers

| Specifiers | Output     | Examples                |
| :-------- | :------- | :------------------------- |
| c         |       character |     x               |
| d or i    | Signed integer  | 1042, -1024         |
| s          | String of characters| Hello Julian
| b         | Binary Representation of unsigned integer| 0101100|
| u         |Unsigned integer| 1024|
| o     | Unsigned octal | 346 |
| x | Unsigned hexadecimal integer | 4ac |
|X | Unsigned hexadecimal integer (uppercase) | 4FF |
| s | String with hex-ascii value replacing special chars | \x0A\x0A |
| p | Pointer address | 0x34596 |
| r | Reversed string of characters | dlroW olleH|

#### flags
| Flag             |    Description                                                              |
| ----------------- | ------------------------------------------------------------------ |
| (-) | Left-justify the output within the field width that was given; Right justification is the default (see width sub-specifier).  | 
| (+) | Preceeds the result with a plus or minus sign (+ or -) even for positive numbers. By default, only negative numbers are preceded with a - sign. |
| (space) | If no sign is going to be written, a blank space is inserted before the value. |
| (#) | Used with o, x or X specifiers the value is preceeded with 0, 0x or 0X respectively for values different than zero. |
|(0) | Left-pads the number with zeroes (0) instead of spaces when padding is specified (see width sub-specifier).

#### width
| Flag             |    Description                                                              |
| ----------------- | ------------------------------------------------------------------ |
| (number) | Minimum number of characters to be printed. If the value to be printed is shorter than this number, the result is padded with blank spaces. The value is not truncated even if the result is larger.  | 
| (*) | The width is not specified in the format string, but as an additional integer value argument preceding the argument that has to be formatted. |

#### Files the repo is having

| Name | Descrption     | Relevant files                |
| :-------- | :------- | :------------------------- |
| README.md        |  It conatains all the information about project      |     none             |
|  man_3_printf | Manual page of our function _printf() | none |
| main.h | Header file with the data type struct, standard libraries and custom prototypes. | *.compilation |
|_printf.c | Main _print functon file. Calls other functions | printf_(name of var).c file |
|functions.c |function first | none |
| functions1.c | second function | none |
|functions2.c | third function | none |
| get_flags.c | flags  | none |
|grt_precision.c |precision | none |
|get_size.c | size | none |
| get_width.c | width  |none |
|handle_print.c | handle function |none|
|utils.c | functions for utils | none |
|write_handlers.c | write file handling function | none |

## **TASKS**

- **0x11. C - printf team project**


0. I'm not going anywhere. You can print that wherever you want to. I'm here and I'm a Spur for life
Write a function that produces output according to a format. You need to handle the following conversion specifiers:
- C
- s
- %

1. Education is when you read the fine print. Experience is what you get if you don' t
Handle the following conversion specifiers:
- d
- i

2. With a face like mine, I do better in print
Handle the following custom conversion specifiers:
- b

3. What one has not experienced, one will never understand in print
Handle the following conversion specifiers:
- u
- o
- x 
- X 

4. Nothing in fine print is ever good news
**Use a local buffer of 1024 chars in order to call write as little as possible.**

5. My weakness is wearing too much leopard print
Handle the following custom conversion specifier:
- s 
- \x 

6. How is the world ruled and led to war? Diplomats lie to journalists and believe t hese lies when they see them in print
**Handle the following conversion specifier: p.**

7. The big print gives and the small print takes away
Handle the following flag characters for non-custom conversion specifiers:

- '+'
- space
- '#'

8. Sarcasm is lost in print
Handle the following length modifiers for non-custom conversion specifiers:
- I
- h conversion specifiers to handle: d, i, u, o, x, X

9. Print some money and give it to us for the rain forests
**Handle the field width for non-custom conversion specifiers.**

10. The negative is the equivalent of the composer's score, and the print the perfor mance
**Handle the precision for non-custom conversion specifiers.**

11. It's depressing when you're still around and your albums are out of print
**Handle the 0 flag character for non-custom conversion specifiers.**

12. Every time that I wanted to give up, if I saw an interesting textile, print what ever, suddenly I would see a collection
**Handle the - flag character for non-custom conversion specifiers.**

13. Print is the sharpest and the strongest weapon of our party
Handle the following custom conversion specifier:
- r:prints the reversed string

14. The flood of print has turned reading into a process of gulping rather than savo ring
Handle the following custom conversion specifier:
- R:prints the rot13'ed string

15. **'*'** 
**All the above options work well together.**
## Run Locally

Clone the project

```bash
  git clone https://ptk@github.com/Deejaht/printf.git
```

Go to the project directory

```bash
  cd printf
```

run, the file is already inside
 - ./a.out

```bash
  ./a.out
```



## Authors

- **Hadijat Abubakar(NIR)** 
- **Aziwe Mlangeni(SA)**

