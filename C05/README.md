# C05 — Recursion & Mathematical Functions

**Day 05 of the 1337 C Piscine**

Iterative and recursive implementations of core mathematical operations. Covers factorial, power, Fibonacci, square root, prime numbers, and the Ten Queens puzzle. No external functions allowed except where noted. **Succeed = 80/100**

## Exercises

### ex00 — `ft_iterative_factorial`
```c
int ft_iterative_factorial(int nb);
```
Iteratively compute and return the factorial of `nb`. Returns `0` if the argument is invalid. Overflow is not handled.

### ex01 — `ft_recursive_factorial`
```c
int ft_recursive_factorial(int nb);
```
Recursively compute and return the factorial of `nb`. Returns `0` if the argument is invalid. Overflow is not handled.

### ex02 — `ft_iterative_power`
```c
int ft_iterative_power(int nb, int power);
```
Iteratively compute and return `nb` raised to `power`. A negative power returns `0`. `0^0 = 1`. Overflow is not handled.

### ex03 — `ft_recursive_power`
```c
int ft_recursive_power(int nb, int power);
```
Recursively compute and return `nb` raised to `power`. A negative power returns `0`. `0^0 = 1`. Overflow is not handled.

### ex04 — `ft_fibonacci`
```c
int ft_fibonacci(int index);
```
Recursively return the nth element of the Fibonacci sequence (0-indexed). The sequence starts: `0, 1, 1, 2, ...`. Returns `-1` if `index` is negative. Overflow is not handled.

### ex05 — `ft_sqrt`
```c
int ft_sqrt(int nb);
```
Return the integer square root of `nb` if it is a perfect square, or `0` if the result would be irrational.

### ex06 — `ft_is_prime`
```c
int ft_is_prime(int nb);
```
Return `1` if `nb` is a prime number, `0` otherwise. Note: `0` and `1` are not prime numbers.

### ex07 — `ft_find_next_prime`
```c
int ft_find_next_prime(int nb);
```
Return the next prime number greater than or equal to `nb`.

## Allowed Functions
| Exercise | Allowed |
|----------|---------|
| ex00 – ex07 | **None** |
| ex08 | **`write`** |

## Compilation
```bash
cc -Wall -Wextra -Werror -o out ft_ten_queens_puzzle.c
```
