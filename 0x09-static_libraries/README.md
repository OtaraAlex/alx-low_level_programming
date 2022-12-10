C - Static libraries
==========================
In this project, I learned what static libraries are and practiced creating and using them with ar, ranlib, and nm.

Concepts
--------

*For this project, students are expected to look at this concept:*

-   [C static libraries](https://alx-intranet.hbtn.io/concepts/61)

Resources
---------

**Read or watch**:

-   [What Is A "C" Library? What Is It Good For?](https://alx-intranet.hbtn.io/rltoken/XB1iH0qE6gshx0x8TfRAPQ "What Is A "C" Library? What Is It Good For?")
-   [Creating A Static "C" Library Using "ar" and "ranlib"](https://alx-intranet.hbtn.io/rltoken/XB1iH0qE6gshx0x8TfRAPQ "Creating A Static "C" Library Using "ar" and "ranlib"")
-   [Using A "C" Library In A Program](https://alx-intranet.hbtn.io/rltoken/XB1iH0qE6gshx0x8TfRAPQ "Using A "C" Library In A Program")
-   [What is difference between Dynamic and Static library(Static and Dynamic linking)](https://alx-intranet.hbtn.io/rltoken/PexOGO-npR_ZDQk-SpOR9g "What is difference between Dynamic and Static library(Static and Dynamic linking)") (*stop at 4:44*)

## Tasks :page_with_curl:

* **0. A library is not a luxury but one of the necessities of life**
  * [libmy.a](./libmy.a): C Static library containing all the functions
  listed below :
    * `int _putchar(char c);`
    * `int _islower(int c);`
    * `int _isalpha(int c);`
    * `int _abs(int n);`
    * `int _isupper(int c);`
    * `int _isdigit(int c);`
    * `int _strlen(char *s);`
    * `void _puts(char *s);`
    * `char *_strcpy(char *dest, char *src);`
    * `int _atoi(char *s);`
    * `char *_strcat(char *dest, char *src);`
    * `char *_strncat(char *dest, char *src, int n);`
    * `char *_strncpy(char *dest, char *src, int n);`
    * `int _strcmp(char *s1, char *s2);`
    * `char *_memset(char *s, char b, unsigned int n);`
    * `char *_memcpy(char *dest, char *src, unsigned int n);`
    * `char *_strchr(char *s, char c);`
    * `unsigned int _strspn(char *s, char *accept);`
    * `char *_strpbrk(char *s, char *accept);`
    * `char *_strstr(char *haystack, char *needle);`

* [main.h](./main.h): Header file containing the prototypes of all functions
  included in `libmy.a`.

* **1. Without libraries what have we? We have no past and no future**
  * [create_static_lib.sh](./create_static_lib.sh): Bash script that creates a static
  library called `liball.a` from all the `.c` files in the current directory.
