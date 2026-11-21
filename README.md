*This project has been created as part of the 42 curriculum by aalrofat.*

# 🖨️ ft_printf

## 📝 Description
The **ft_printf** project is a custom re-implementation of the standard C `printf` function, designed to format and output data to the standard output (`stdout`) based on conversion specifiers. It supports variadic arguments to handle a variable number of inputs cleanly and accurately while returning the total count of printed characters.

### 💡 What did I learn from the project
Building **ft_printf** taught me how variadic functions work in C using `<stdarg.h>` (`va_start`, `va_arg`, `va_end`). I also practiced parsing format strings, handling different data types and base conversions (such as hexadecimal and unsigned integers), and maintaining clean modular structure following the Norminette.

## ⚙️ Instructions
1. `cd ft_printf` (or navigate to the project directory)
2. `make` (compiles object files and creates `libftprintf.a`)
3. **Useful Makefile rules**:
   - `make clean` : Removes object files (`.o`).
   - `make fclean` : Removes object files and `libftprintf.a`.
   - `make re` : Rebuilds the library from scratch.
4. **Usage in a C project**: Include `ft_printf.h` and link `libftprintf.a` during compilation, for example:
   - `cc -Wall -Wextra -Werror main.c libftprintf.a -o printf_test`

## 🛠️ Supported Conversions
- `%c` : Prints a single character.
- `%s` : Prints a string.
- `%p` : Prints a `void *` pointer address in hexadecimal format.
- `%d` / `%i` : Prints a signed decimal / integer.
- `%u` : Prints an unsigned decimal integer.
- `%x` / `%X` : Prints a number in lowercase / uppercase hexadecimal format.
- `%%` : Prints a percent sign.

## 🔗 Resources
- [Linux man pages: printf(3)](https://man7.org/linux/man-pages/man3/printf.html)
- [Linux man pages: stdarg(3)](https://man7.org/linux/man-pages/man3/stdarg.3.html)
- [42 Norminette](https://github.com/42School/norminette)

### 🤖 AI Usage
- **Explaining Concepts**: Helped clarify variadic argument macros (`va_list`, `va_start`, `va_arg`, `va_end`) and base formatting edge cases.
- **Code Organization**: Helped structure format dispatchers and helper functions cleanly according to the Norminette.
- **Documentation**: Helped draft and refine the English in this README file.
