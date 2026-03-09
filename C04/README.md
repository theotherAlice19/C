# C04 — Number Conversion & Base Systems

**Day 04 of the 1337 C Piscine**

Number to string, string to number, and custom base arithmetic. Introduces `write`, `atoi`, and base conversion. The validation threshold is **Succeed = 70/100**.

## Exercises

### ex00 — `ft_strlen`
```c
int ft_strlen(char *str);
```
Count and return the number of characters in a string, not including the null terminator.

### ex01 — `ft_putstr`
```c
void ft_putstr(char *str);
```
Display a string of characters on standard output using `write`.

### ex02 — `ft_putnbr`
```c
void ft_putnbr(int nb);
```
Display an integer on standard output. Must handle all `int` values including `INT_MIN` (-2147483648) and `INT_MAX` (2147483647).

Example: `ft_putnbr(42)` displays `42`.

### ex03 — `ft_atoi`
```c
int ft_atoi(char *str);
```
Convert the initial portion of a string to its `int` representation, mimicking standard `atoi` with extensions:
- Skips leading whitespace (`' '`, `'\t'`, `'\n'`, `'\r'`, `'\f'`, `'\v'`)
- Handles any number of `+` and `-` signs (odd number of `-` = negative result)
- Reads digits until a non-digit character is found
- No overflow handling required

Example:
```
"   ---+--+1234ab567" → -1234
```

## Allowed Functions
| Exercise | Allowed |
|----------|---------|
| ex00 | **None** |
| ex01, ex02, ex04 | **`write`** |
| ex03, ex05 | **None** |

## Compilation
```bash
cc -Wall -Wextra -Werror -o out ft_putnbr_base.c
```
