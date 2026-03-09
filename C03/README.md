# C03 — String Comparison & Concatenation

**Day 03 of the 1337 C Piscine**
String comparison and concatenation from scratch. No standard library allowed. The validation threshold is **Succeed = 50/100**.

## Exercises

### ex00 — `ft_strcmp`
```c
int ft_strcmp(char *s1, char *s2);
```
Reproduce the behavior of `strcmp`. Compare two strings character by character and return the difference of the first differing characters (as `unsigned char`). Returns `0` if strings are equal.

### ex01 — `ft_strncmp`
```c
int ft_strncmp(char *s1, char *s2, unsigned int n);
```
Reproduce the behavior of `strncmp`. Same as `ft_strcmp` but compares at most `n` characters. Returns `0` if `n` is `0`.

### ex02 — `ft_strcat`
```c
char *ft_strcat(char *dest, char *src);
```
Reproduce the behavior of `strcat`. Appends `src` to the end of `dest`, overwriting `dest`'s null terminator. Always null-terminates. Returns `dest`.

### ex03 — `ft_strncat`
```c
char *ft_strncat(char *dest, char *src, unsigned int nb);
```
Reproduce the behavior of `strncat`. Appends at most `nb` characters from `src` to `dest`, then null-terminates. Returns `dest`.

## Allowed Functions
| Exercise | Allowed |
|----------|---------|
| ex00–ex05 | **None** |

## Compilation
```bash
cc -Wall -Wextra -Werror -o out ft_strcmp.c
```

