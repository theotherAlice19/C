# C01 — Pointers & Arrays

**Day 01 of the 1337 C Piscine**

Introduction to pointers, pass-by-address, basic string handling, and array manipulation. The validation threshold is **Succeed = 100/100**.

## Exercises

### ex00 — `ft_ft`
```c
void ft_ft(int *nbr);
```
Takes a pointer to `int` as parameter and sets its value to `42`.
First introduction to dereferencing a pointer to modify a variable.

### ex01 — `ft_ultimate_ft`
```c
void ft_ultimate_ft(int *********nbr);
```
Same as `ft_ft` but the pointer is **9 levels deep** (`int *********`).
Dereference all 9 levels and set the final `int` to `42`.

### ex02 — `ft_swap`
```c
void ft_swap(int *a, int *b);
```
Swap the values of two integers using their addresses.
Classic pass-by-pointer pattern — essential for understanding why pass-by-value doesn't work here.

### ex03 — `ft_div_mod`
```c
void ft_div_mod(int a, int b, int *div, int *mod);
```
Divide `a` by `b`:
- Store the **quotient** in `*div`
- Store the **remainder** in `*mod`

### ex04 — `ft_ultimate_div_mod`
```c
void ft_ultimate_div_mod(int *a, int *b);
```
Divide `*a` by `*b`:
- Store the **quotient** back into `*a`
- Store the **remainder** back into `*b`

### ex05 — `ft_putstr`
```c
void ft_putstr(char *str);
```
Display a string of characters to standard output using `write`.
Iterate through the char array until `'\0'`.

### ex06 — `ft_strlen`
```c
int ft_strlen(char *str);
```
Count and return the number of characters in a string (not counting the null terminator).

### ex07 — `ft_rev_int_tab`
```c
void ft_rev_int_tab(int *tab, int size);
```
Reverse an array of integers in-place. First element becomes last, last becomes first.

### ex08 — `ft_sort_int_tab`
```c
void ft_sort_int_tab(int *tab, int size);
```
Sort an array of integers by ascending order in-place.

## Allowed Functions

| Exercise | Allowed |
|----------|---------|
| ex00–ex04, ex06–ex08 | **None** |
| ex05 | **`write`** |

## Compilation
```bash
cc -Wall -Wextra -Werror -o out ft_swap.c
```
