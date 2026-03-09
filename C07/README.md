# C07 — Dynamic Memory Allocation

**Day 07 of the 1337 C Piscine**

First contact with `malloc`. Building functions that allocate memory on the heap to duplicate strings, generate integer ranges, join string arrays, convert bases, and split strings. **Succeed = 60/100**

## Exercises

### ex00 — `ft_strdup`
```c
char *ft_strdup(char *src);
```
Reproduce the behavior of the standard `strdup` function. Allocates sufficient memory for a copy of `src`, copies it, and returns a pointer to the duplicate.

### ex01 — `ft_range`
```c
int *ft_range(int min, int max);
```
Allocate and return an array of ints containing all values from `min` (included) to `max` (excluded). Returns `NULL` if `min >= max`.

### ex02 — `ft_ultimate_range`
```c
int ft_ultimate_range(int **range, int min, int max);
```
Same as `ft_range` but assigns the allocated array through the `range` pointer parameter instead of returning it. Returns the size of the range, `0` if `min >= max` (with `*range` set to `NULL`), or `-1` on allocation error.

### ex03 — `ft_strjoin`
```c
char *ft_strjoin(int size, char **strs, char *sep);
```
Concatenate all `size` strings from `strs` into a single newly allocated string, with `sep` inserted between each. If `size` is `0`, returns an empty freeable string.

## Allowed Functions
| Exercise | Allowed |
|----------|---------|
| ex00 – ex03, ex05 | **`malloc`** |
| ex04 | **`malloc`**, **`free`** |

## Compilation
```bash
cc -Wall -Wextra -Werror -o out ft_split.c
```
