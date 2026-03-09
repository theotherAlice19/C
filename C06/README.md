# C06 — Command-Line Arguments

**Day 06 of the 1337 C Piscine**

Introduction to `argc` and `argv`. Programs that read, display, reverse, and sort their command-line arguments. All exercises require a `main` function and are standalone programs. **Succeed = 100/100**

## Exercises

### ex00 — `ft_print_program_name`
```c
int main(int argc, char **argv);
```
A program that displays its own name followed by a newline.

Example:
```
$>./a.out | cat -e
./a.out$
$>
```

### ex01 — `ft_print_params`
```c
int main(int argc, char **argv);
```
A program that displays each of its arguments on a separate line, in the same order as provided on the command line. `argv[0]` is not displayed.

Example:
```
$>./a.out test1 test2 test3 | cat -e
test1$
test2$
test3$
$>
```

### ex02 — `ft_rev_params`
```c
int main(int argc, char **argv);
```
A program that displays each of its arguments on a separate line, in reverse order. `argv[0]` is not displayed.

### ex03 — `ft_sort_params`
```c
int main(int argc, char **argv);
```
A program that displays each of its arguments on a separate line, sorted in ASCII order. `argv[0]` is not displayed.

## Allowed Functions
| Exercise | Allowed |
|----------|---------|
| ex00 – ex03 | **`write`** |

## Compilation
```bash
cc -Wall -Wextra -Werror -o a.out ft_sort_params.c
```
