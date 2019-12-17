# 42-libft
School 42 project - [Libft](libft.en.pdf).
# Table of Contents
* [Part 1 - Libc functions](#part-1---libc-functions)
  * [ft_memset](#ft_memset)
  * [ft_bzero](#ft_bzero)
  * [ft_memcpy](#ft_memcpy)
  * [ft_memccpy](#ft_memccpy)
  * [ft_memmove](#ft_memmove)
  * [ft_memchr](#ft_memchr)
  * [ft_memcmp](#ft_memcmp)
  * [ft_strlen](#ft_strlen)
  * [ft_strdup](#ft_strdup)
  * [ft_strcpy](#ft_strcpy)
  * [ft_strncpy](#ft_strncpy)
  * [ft_strcat](#ft_strcat)
  * [ft_strncat](#ft_strncat)
  * [ft_strlcat](#ft_strlcat)
  * [ft_strchr](#ft_strchr)
  * [ft_strrchr](#ft_strrchr)
  * [ft_strstr](#ft_strstr)
  * [ft_strnstr](#ft_strnstr)
  * [ft_strcmp](#ft_strcmp)
  * [ft_strncmp](#ft_strncmp)
  * [ft_atoi](#ft_atoi)
  * [ft_isalpha](#ft_isalpha)
  * [ft_isdigit](#ft_isdigit)
  * [ft_isalnum](#ft_isalnum)
  * [ft_isascii](#ft_isascii)
  * [ft_isprint](#ft_isprint)
  * [ft_toupper](#ft_toupper)
  * [ft_tolower](#ft_tolower)
* [Part 2 - Additional functions](#part-2---additional-functions)
  * [ft_memalloc](#ft_memalloc)
  * [ft_memdel](#ft_memdel)
  * [ft_strnew](#ft_strnew)
  * [ft_strdel](#ft_strdel)
  * [ft_strclr](#ft_strclr)
  * [ft_striter](#ft_striter)
  * [ft_striteri](#ft_striteri)
  * [ft_strmap](#ft_strmap)
  * [ft_strmapi](#ft_strmapi)
  * [ft_putnbr](#ft_putnbr)
  * [ft_putchar_fd](#ft_putchar_fd)
  * [ft_putstr_fd](#ft_putstr_fd)
  * [ft_putendl_fd](#ft_putendl_fd)
  * [ft_putnbr_fd](#ft_putnbr_fd)
* [Bonus part](#bonus-part)
# Part 1 - Libc functions
## [ft_memset](ft_memset.c)
`void	*ft_memset(void *str, int c, size_t n)`

Sets the first n bytes of the block of memory pointed by str to the specified value (interpreted as an unsigned char).
### Return Value
Returns a pointer to str.
## [ft_bzero](ft_bzero.c)
`void	ft_bzero(void *str, size_t n)`

Sets the first n bytes of the block of memory pointed by str to zero.
### Return Value
None.
## [ft_memcpy](ft_memcpy.c)
`void	*ft_memcpy(void *dest, const void *src, size_t n)`

Copies n bytes from memory area src to memory area dest. The memory areas must not overlap. Use **[ft_memmove](#ft_memmove)** if the memory areas do overlap.
### Return Value
Returns a pointer to dest.
## [ft_memccpy](ft_memccpy.c)
`void	*ft_memccpy(void *dest, const void *src, int c, size_t n)`

Copies no more than n bytes from memory area src to memory area dest, stopping when the character c is found. If the memory areas overlap, the results are undefined.
### Return Value
Returns a pointer to the next character in dest after c, or NULL if c was not found in the first n characters of src.
## [ft_memmove](ft_memmove.c)
`void	*ft_memmove(void *dest, const void *src, size_t n)`

Copies n bytes from memory area src to memory area dest. The memory areas may overlap.
### Return Value
Returns a pointer to dest.
## [ft_memchr](ft_memchr.c)
`void *ft_memchr(const void *str, int c, size_t n)`

Scans the initial n bytes of the memory area pointed to by str for the first instance of c. Both c and the bytes of the memory area pointed to by str are interpreted as unsigned char.
### Return Value
Returns a pointer to the matching byte or NULL if the character does not occur in the given memory area.
## [ft_memcmp](ft_memcmp.c)
`int ft_memcmp(const void *buf1, const void *buf2, size_t n)`

Compares the first n bytes (each interpreted as unsigned char) of the memory areas buf1 and buf2.
### Return Value
Returns an integer less than, equal to, or greater than zero if the first n bytes of buf1 is found, respectively, to be less than, to match, or be greater than the first n bytes of buf2.
For a nonzero return value, the sign is determined by the sign of the difference between the first pair of bytes (interpreted as unsigned char) that differ in buf1 and buf2.
## [ft_strlen](ft_strlen.c)
`size_t	ft_strlen(const char *str)`

Calculates the length of the string str, excluding the terminating null byte.
### Return Value
Returns the number of bytes in the string str.
## [ft_strdup](ft_strdup.c)
Returns a pointer to a new string which is a duplicate of the string s. Memory for the new string is obtained with **malloc**, and can be freed with **free**.
### Return Value
Returns a pointer to the duplicated string, or NULL if insufficient memory was available.
## [ft_strcpy](ft_strcpy.c)
`char *ft_strcpy(char *str1, const char *str2)`

[description]
### Return Value
[return_value]
## [ft_strncpy](ft_strncpy.c)
`char *ft_strncpy(char *dest, const char *src, size_t n)`

[description]
### Return Value
[return_value]
## [ft_strcat](ft_strcat.c)
`char *ft_strcat(char *s1, const char *s2)`

[description]
### Return Value
[return_value]
## [ft_strncat](ft_strncat.c)
`char *ft_strncat(char *s1, const char *s2, size_t n)`

[description]
### Return Value
[return_value]
## [ft_strlcat](ft_strlcat.c)
`size_t ft_strlcat(char *dst, const char *src, size_t dstsize)`

[description]
### Return Value
[return_value]
## [ft_strchr](ft_strchr.c)
`char *ft_strchr(const char *s, int c)`

[description]
### Return Value
[return_value]
## [ft_strrchr](ft_strrchr.c)
`char *ft_strrchr(const char *s, int c)`

[description]
### Return Value
[return_value]
## [ft_strstr](ft_strstr.c)
`char *ft_strstr(const char *s1, const char *s2)`

[description]
### Return Value
[return_value]
## [ft_strnstr](ft_strnstr.c)
`char *ft_strnstr(const char *s1, const char *s2, size_t len)`

[description]
### Return Value
[return_value]
## [ft_strcmp](ft_strcmp.c)
`int ft_strcmp(const char *str1, const char *str2)`

[description]
### Return Value
[return_value]
## [ft_strncmp](ft_strncmp.c)
`int ft_strncmp(const char *s1, const char *s2, size_t n)`

[description]
### Return Value
[return_value]
## [ft_atoi](ft_atoi.c)
`int ft_atoi(const char *str)`

[description]
### Return Value
[return_value]
## [ft_isalpha](ft_isalpha.c)
`int ft_isalpha(int c)`

[description]
### Return Value
[return_value]
## [ft_isdigit](ft_isdigit.c)
`int ft_isdigit(int c)`

[description]
### Return Value
[return_value]
## [ft_isalnum](ft_isalnum.c)
`int ft_isalnum(int c)`

[description]
### Return Value
[return_value]
## [ft_isascii](ft_isascii.c)
`int ft_isascii(int c)`

[description]
### Return Value
[return_value]
## [ft_isprint](ft_isprint.c)
`int ft_isprint(int c)`

[description]
### Return Value
[return_value]
## [ft_toupper](ft_toupper.c)
`int ft_toupper(int c)`

[description]
### Return Value
[return_value]
## [ft_tolower](ft_tolower.c)
`int ft_tolower(int c)`

[description]
### Return Value
[return_value]
# Part 2 - Additional functions
## [ft_memalloc](ft_memalloc.c)
`void * ft_memalloc(size_t size)`

Allocates with **malloc** and returns a "fresh" memory area. The memory allocated is initialized to 0. If the allocation fails, the function returns NULL.
### Return Value
Returns the allocated memory area.
## [ft_memdel](ft_memdel.c)
`void ft_memdel(void **ap)`

Takes as a parameter the address of a memory area that needs to be freed with **free**, then puts the pointer to NULL.
### Return Value
None.
## [ft_strnew](ft_strnew.c)
`char * ft_strnew(size_t size)`

Allocates with **malloc** and returns a "fresh" string ending with '\0'. Each character of the string is initialized at
'\0'. If the allocation fails the function returns NULL.
### Return Value
Returns the string allocated and initialized to 0.
## [ft_strdel](ft_strdel.c)
`void ft_strdel(char **as)`

Takes as a parameter the address of a string that need to be freed with **free**, then sets its pointer to NULL.
### Return Value
None.
## [ft_strclr](ft_strclr.c)
`void ft_strclr(char *s)`

Sets every character of the string to the value '\0'.
### Return Value
None.
## [ft_striter](ft_striter.c)
`void ft_striter(char *s, void (*f)(char *))`

Applies the function f to each character of the string passed as argument. Each character is passed by address to f to be modified if necessary.
### Return Value
None.
## [ft_striteri](ft_striteri.c)
`void ft_striteri(char *s, void (*f)(unsigned int, char *))`

Applies the function f to each character of the string passed as argument, and passing its index as first argument. Each character is passed by address to f to be modified if necessary.
### Return Value
None.
## [ft_strmap](ft_strmap.c)
`char * ft_strmap(char const *s, char (*f)(char))`

Applies the function f to each character of the string given as argument to create a "fresh" new string with **malloc** resulting from the successive applications of f.
### Return Value
Returns the "fresh" string created from the successive applications of f.
## [ft_strmapi](ft_strmapi.c)
`char * ft_strmapi(char const *s, char (*f)(unsigned int, char))`

Applies the function f to each character of the string passed as argument by giving its index as first argument to create a "fresh" new string with **malloc** resulting from the successive applications of f.
### Return Value
Returns the "fresh" string created from the successive applications of f.
## [ft_putnbr](ft_putnbr.c)
`void ft_putnbr(int n)`

Outputs the integer n to the standard output.
### Return Value
None.
## [ft_putchar_fd](ft_putchar_fd.c)
`void ft_putchar_fd(char c, int fd)`

Outputs the char c to the file descriptor fd.
### Return Value
None.
## [ft_putstr_fd](ft_putstr_fd.c)
`void ft_putstr_fd(char const *s, int fd)`

Outputs the string s to the file descriptor fd.
### Return Value
None.
## [ft_putendl_fd](ft_putendl_fd.c)
`void ft_putendl_fd(char const *s, int fd)`

Outputs the string s to the file descriptor fd followed by a '\n'.
### Return Value
None.
## [ft_putnbr_fd](ft_putnbr_fd.c)
`void ft_putnbr_fd(int n, int fd)`

Outputs the integer n to the file descriptor fd.
### Return Value
None.
# Bonus part
