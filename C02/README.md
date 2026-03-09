# C02 — String Manipulation

**Day 02 of the 1337 C Piscine**
Deep dive into string handling: copying, validating, transforming case, and inspecting raw memory. The validation threshold is **Succeed = 85/100**.

## Exercises

### ex00 — `ft_strcpy`
```c
char *ft_strcpy(char *dest, char *src);
```
Reproduce the behavior of `strcpy`. Copy `src` into `dest` including the null terminator. Return `dest`.

### ex01 — `ft_strncpy`
```c
char *ft_strncpy(char *dest, char *src, unsigned int n);
```
Reproduce the behavior of `strncpy`. Copy at most `n` characters from `src` to `dest`. If `src` is shorter than `n`, pad `dest` with null bytes.

### ex02 — `ft_str_is_alpha`
```c
int ft_str_is_alpha(char *str);
```
Return `1` if the string contains **only alphabetical characters**, `0` otherwise.
Returns `1` if `str` is empty.

### ex03 — `ft_str_is_numeric`
```c
int ft_str_is_numeric(char *str);
```
Return `1` if the string contains **only digit characters** (`0`–`9`), `0` otherwise.
Returns `1` if `str` is empty.

### ex04 — `ft_str_is_lowercase`
```c
int ft_str_is_lowercase(char *str);
```
Return `1` if the string contains **only lowercase letters**, `0` otherwise.
Returns `1` if `str` is empty.

### ex05 — `ft_str_is_uppercase`
```c
int ft_str_is_uppercase(char *str);
```
Return `1` if the string contains **only uppercase letters**, `0` otherwise.
Returns `1` if `str` is empty.

### ex06 — `ft_str_is_printable`
```c
int ft_str_is_printable(char *str);
```
Return `1` if the string contains **only printable characters** (ASCII 32–126), `0` otherwise.
Returns `1` if `str` is empty.

### ex07 — `ft_strupcase`
```c
char *ft_strupcase(char *str);
```
Convert every letter in the string to **uppercase**. Non-letter characters are unchanged. Returns `str`.

### ex08 — `ft_strlowcase`
```c
char *ft_strlowcase(char *str);
```
Convert every letter in the string to **lowercase**. Non-letter characters are unchanged. Returns `str`.

### ex09 — `ft_strcapitalize`
```c
char *ft_strcapitalize(char *str);
```
Capitalize the **first letter of each word** and lowercase all other letters.
A "word" is a sequence of alphanumeric characters — punctuation and spaces act as separators.

Example:
```
"salut, comment tu vas ? 42mots quarante-deux; cinquante+et+un"
→ "Salut, Comment Tu Vas ? 42mots Quarante-Deux; Cinquante+Et+Un"
```

### ex10 — `ft_strlcpy`
```c
unsigned int ft_strlcpy(char *dest, char *src, unsigned int size);
```
Reproduce `strlcpy`. Copy at most `size - 1` characters from `src` to `dest` and always null-terminate. Returns the total length of `src`.

### ex11 — `ft_putstr_non_printable`
```c
void ft_putstr_non_printable(char *str);
```
Display a string. Non-printable characters are shown as `\xx` where `xx` is their **lowercase hexadecimal** value.

Example: `"Coucou\ntu"` → displays `Coucou\0atu`

## Allowed Functions

| Exercise | Allowed |
|----------|---------|
| ex00–ex10 | **None** |
| ex11, ex12 | **`write`** |

## Compilation
```bash
cc -Wall -Wextra -Werror -o out ft_strcpy.c
```
