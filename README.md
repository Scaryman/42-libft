# 42 Libft
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
  * [ft_strequ](#ft_strequ)
  * [ft_strnequ](#ft_strnequ)
  * [ft_strsub](#ft_strsub)
  * [ft_strjoin](#ft_strjoin)
  * [ft_strtrim](#ft_strtrim)
  * [ft_strsplit](#ft_strsplit)
  * [ft_itoa](#ft_itoa)
  * [ft_putchar](#ft_putchar)
  * [ft_putstr](#ft_putstr)
  * [ft_putendl](#ft_putendl)
  * [ft_putnbr](#ft_putnbr)
  * [ft_putchar_fd](#ft_putchar_fd)
  * [ft_putstr_fd](#ft_putstr_fd)
  * [ft_putendl_fd](#ft_putendl_fd)
  * [ft_putnbr_fd](#ft_putnbr_fd)
* [Bonus part](#bonus-part)
  * [ft_lstnew](#ft_lstnew)
  * [ft_lstdelone](#ft_lstdelone)
  * [ft_lstdel](#ft_lstdel)
  * [ft_lstadd](#ft_lstadd)
  * [ft_lstiter](#ft_lstiter)
  * [ft_lstmap](#ft_lstmap)
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
## [ft_strequ](ft_strequ.c)
`int ft_strequ(char const *s1, char const *s2)`

Lexicographical comparison between s1 and s2. If the 2 strings are identical the function returns 1, or 0 otherwise.
### Return Value
Returns 1 or 0 according to if the 2 strings are identical or not.
## [ft_strnequ](ft_strnequ.c)
`int ft_strnequ(char const *s1, char const *s2, size_t n)`

Lexicographical comparison between s1 and s2 up to n characters or until a '\0' is reached. If the 2 strings are identical, the function returns 1, or 0 otherwise.
### Return Value
Returns 1 or 0 according to if the 2 strings are identical or not.
## [ft_strsub](ft_strsub.c)
`char * ft_strsub(char const *s, unsigned int start, size_t len)`

Allocates with **malloc** and returns a "fresh" substring from the string given as argument. The substring begins at indexstart and is of size len. If start and len aren’t refering to a valid substring, the behavior is undefined. If the allocation fails, the function returns NULL.
### Return Value
Returns the substring.
## [ft_strjoin](ft_strjoin.c)
`char * ft_strjoin(char const *s1, char const *s2)`

Allocates with **malloc** and returns a “fresh” string ending with ’\0’, result of the concatenation of s1 and s2. If the allocation fails the function returns NULL.
### Return Value
Returns the "fresh" string result of the concatenation of the 2 strings.
## [ft_strtrim](ft_strtrim.c)
`char * ft_strtrim(char const *s)`

Allocates with **malloc** and returns a copy of the string given as argument without whitespaces at the beginning or at the end of the string. Will be considered as whitespaces the following characters ' ', '\n' and '\t'. If s has no whitespaces at the beginning or at the end, the function returns a copy of s. If the allocation fails the function returns NULL.
### Return Value
Returns the "fresh" trimmed string or a copy of s.
## [ft_strsplit](ft_strsplit.c)
`char ** ft_strsplit(char const *s, char c)`

Allocates with **malloc** and returns an array of "fresh" strings (all ending with '\0', including the array itself) obtained by spliting s using the character c as a delimiter. If the allocation fails the function returns NULL.
### Return Value
Returns the array of "fresh" strings result of the split.
## [ft_itoa](ft_itoa.c)
`char * ft_itoa(int n)`

Allocate with **malloc** and returns a "fresh" string ending with '\0' representing the integer n given as argument. Negative numbers must be supported. If the allocation fails, the function returns NULL.
### Return Value
Returns the string representing the integer passed as argument.
## [ft_putchar](ft_putchar.c)
`void ft_putchar(char c)`

Outputs the character c to the standard output.
### Return Value
None.
## [ft_putstr](ft_putstr.c)
`void ft_putstr(char const *s)`

Outputs the string s to the standard output.
### Return Value
None.
## [ft_putendl](ft_putendl.c)
`void ft_putendl(char const *s)`

Outputs the string s to the standard output followed by a '\n'.
### Return Value
None.
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
## [ft_lstnew](ft_lstnew.c)
`t_list * ft_lstnew(void const *content, size_t content_size)`

Allocates with **malloc** and returns a "fresh" link. The variables content and content_size of the new link are initialized by copy of the parameters of the function. If the parameter content is nul, the variable content is initialized to NULL and the variable content_size is initialized to 0 even if the parameter content_size isn’t. The variable next is initialized to NULL. If the allocation fails, the function returns NULL.
### Return Value
Returns the new list.
## [ft_lstdelone](ft_lstdelone.c)
`void ft_lstdelone(t_list **alst, void (*del)(void *, size_t))`

Takes as a parameter a link’s pointer address and frees the memory of the link’s content using the function del given as a parameter, then frees the link’s memory using **free**. The memory of next must not be freed under any circumstance. Finally, the pointer to the link that was just freed must be set to NULL (quite similar to the function ft_memdel in the mandatory part).
### Return Value
None.
## [ft_lstdel](ft_lstdel.c)
`void ft_lstdel(t_list **alst, void (*del)(void *, size_t))`

Takes as a parameter the adress of a pointer to a link and frees the memory of this link and every successors of that link using the functions del and free(3). Finally the pointer to the link that was just freed must be set to NULL (quite similar to the function ft_memdel from the mandatory part).
### Return Value
None.
## [ft_lstadd](ft_lstadd.c)
`void ft_lstadd(t_list **alst, t_list *new)`

Adds the element new at the beginning of the list.
### Return Value
None.
## [ft_lstiter](ft_lstiter.c)
`void ft_lstiter(t_list *lst, void (*f)(t_list *elem))`

Iterates the list lst and applies the function f to each link.
### Return Value
None.
## [ft_lstmap](ft_lstmap.c)
`t_list * ft_lstmap(t_list *lst, t_list * (*f)(t_list *elem))`

Iterates a list lst and applies the function f to each link to create a “fresh” list (using malloc(3)) resulting from the successive applications of f. If the allocation fails, the function returns NULL.
### Return Value
Returns the new list.
