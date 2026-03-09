# C00 — Basic Output & Combinations

**Day 00 of the 1337 C Piscine**

First contact with C: using `write()` directly, printing characters, digits, and generating combinations with nested loops. **Succeed = 85/100**

## Exercises

### ex00 — `ft_putchar`
```c
void ft_putchar(char c);
```
Write a function that displays a single character using `write(1, &c, 1)`.
The most fundamental building block — everything else is built on top of this.

### ex01 — `ft_print_alphabet`
```c
void ft_print_alphabet(void);
```
Display the entire lowercase alphabet on a single line, from `'a'` to `'z'`.

### ex02 — `ft_print_reverse_alphabet`
```c
void ft_print_reverse_alphabet(void);
```
Display the alphabet in lowercase from `'z'` down to `'a'` on a single line.

### ex03 — `ft_print_numbers`
```c
void ft_print_numbers(void);
```
Display all digits from `'0'` to `'9'` on a single line, in ascending order.

### ex04 — `ft_is_negative`
```c
void ft_is_negative(int n);
```
Display `'N'` if `n` is negative, `'P'` if `n` is zero or positive.

### ex05 — `ft_print_comb`
```c
void ft_print_comb(void);
```
Display all unique combinations of **3 different digits** in ascending order, separated by `, `.

Expected output:
```
012, 013, 014, ..., 789
```
- `789` appears but `987` doesn't — each combo is sorted and unique.
- No digit repeats within a combo (`999` is excluded).

### ex06 — `ft_print_comb2`
```c
void ft_print_comb2(void);
```
Display all unique combinations of **two 2-digit numbers** between `00` and `99`, in ascending order.

Expected output:
```
00 01, 00 02, ..., 00 99, 01 02, ..., 98 99
```
### ex07 — `ft_putnbr`
```c
void ft_putnbr(int nb);
```
Display an integer — must handle **all possible `int` values**, including `INT_MIN` (`-2147483648`).

### ex08 — `ft_print_combn`
```c
void ft_print_combn(int n);
```
Generalization of `ft_print_comb`: display all unique combinations of `n` different digits in ascending order. `n` is guaranteed to satisfy `0 < n < 10`.

For `n = 2`:
```
01, 02, 03, ..., 09, 12, ..., 79, 89
```

## Allowed Functions
All exercises in C00 only allow: **`write`**

## Compilation
```bash
cc -Wall -Wextra -Werror -o out ft_putchar.c
```

