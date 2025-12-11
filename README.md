# 📚 Libft - Your Very First Own C Library

**Libft** is the first project in the **42 School** Common Core curriculum. It is a custom-made standard C library that reimplements many standard C library functions (`libc`) and introduces additional utility functions.

The goal is to understand how these standard functions work under the hood, learn about memory management, and build a reusable library that will be used in future 42 projects.

## 🚀 Features

* **Standard Libc Functions:** Custom implementation of standard C functions like `strlen`, `memset`, `atoi`, etc.
* **Additional Utilities:** Useful functions for string manipulation, file descriptor output, and linked list handling.
* **Bonus Part:** Functions to manipulate singly linked lists.
* **Custom Extensions:** Includes functions for matrix handling, `get_next_line`, and `ft_printf`.

---

## 🛠️ Function Overview

### 1. String Manipulation (`string_functions/`)
Functions to analyze and transform strings.
* `ft_strlen` - Calculate string length.
* `ft_strlcpy`, `ft_strlcat` - Safer string copy and concatenation.
* `ft_strchr`, `ft_strrchr` - Locate character in string.
* `ft_strnstr` - Locate a substring in a string.
* `ft_strncmp` - Compare two strings.
* `ft_strdup` - Duplicate a string using `malloc`.
* `ft_substr` - Extract a substring from a string.
* `ft_strjoin` - Concatenate two strings into a new one.
* `ft_strtrim` - Trim characters from the beginning and end of a string.
* `ft_split` - Split a string into an array of strings using a delimiter.
* `ft_strmapi`, `ft_striteri` - Apply a function to every character of a string.

### 2. Memory Management (`memory_functions/`)
Functions to manipulate raw memory blocks.
* `ft_memset` - Fill memory with a constant byte.
* `ft_bzero` - Zero a byte string.
* `ft_memcpy` - Copy memory area.
* `ft_memmove` - Copy memory area (safe for overlapping regions).
* `ft_memchr` - Scan memory for a character.
* `ft_memcmp` - Compare memory areas.
* `ft_calloc` - Allocate memory and set it to zero.
* `ft_realloc` - Reallocate memory block (custom addition).

### 3. Character Checks & Conversions
* `ft_isalpha`, `ft_isdigit`, `ft_isalnum`, `ft_isascii`, `ft_isprint` - Character classification.
* `ft_toupper`, `ft_tolower` - Character case conversion.

### 4. Integer & Conversion Functions (`int_functions/`)
* `ft_atoi`, `ft_atol` - Convert string to integer/long.
* `ft_itoa` - Convert integer to string.
* `ft_putnbr_fd` - Output integer to a file descriptor.

### 5. Linked List Functions (`list_functions/`)
Functions to manipulate singly linked lists (`t_list`).
* `ft_lstnew` - Create a new list node.
* `ft_lstadd_front` - Add a node to the beginning of the list.
* `ft_lstadd_back` - Add a node to the end of the list.
* `ft_lstsize` - Count the number of nodes in a list.
* `ft_lstlast` - Retrieve the last node of the list.
* `ft_lstdelone` - Delete a single node.
* `ft_lstclear` - Delete and free a sequence of nodes.
* `ft_lstiter` - Apply a function to the content of each node.
* `ft_lstmap` - Apply a function to each node and create a new list.

### 6. Matrix & Custom Utilities (`matrix_functions/` & others)
* `ft_split` - Splits a string into a matrix.
* `ft_matrix_len` - Returns the length of a matrix.
* `ft_dup_matrix` - Duplicates a double pointer array.
* `ft_free_matrix` - Frees a dynamically allocated matrix.
* **Get_next_line:** Reads a line from a file descriptor.
* **Ft_printf:** Formats and prints data.

---

## 💻 Installation & Usage

### Compilation
To compile the library, run:

```bash
make
This will generate the libft.a static library file.

Using it in your code
Include the header file in your C files:
#include "libft.h"
cc main.c -L. -lft -o my_program
```

```text
📂 Project Structure
libft/
├── Makefile
├── libft.h
├── int_functions/       # Integer manipulation (atoi, itoa, putnbr...)
├── list_functions/      # Linked list manipulation (lstnew, lstadd...)
├── matrix_functions/    # Matrix manipulation (split, free_matrix...)
├── memory_functions/    # Memory manipulation (memset, calloc...)
└── string_functions/    # String manipulation (strlen, strdup...)

