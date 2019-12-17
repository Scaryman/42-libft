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
# Part 1 - Libc functions
## ft_memset
`void	*ft_memset(void *str, int c, size_t n)`

Sets the first n bytes of the block of memory pointed by str to the specified value (interpreted as an unsigned char).
### Return Value
Returns a pointer to str.
## ft_bzero
`void	ft_bzero(void *str, size_t n)`

Sets the first n bytes of the block of memory pointed by str to zero.
### Return Value
None.
## ft_memcpy
`void	*ft_memcpy(void *dest, const void *src, size_t n)`

Copies n bytes from memory area src to memory area dest. The memory areas must not overlap. Use **[ft_memmove](#ft_memmove)** if the memory areas do overlap.
### Return Value
Returns a pointer to dest.
## ft_memccpy
`void	*ft_memccpy(void *dest, const void *src, int c, size_t n)`

Copies no more than n bytes from memory area src to memory area dest, stopping when the character c is found. If the memory areas overlap, the results are undefined.
### Return Value
Returns a pointer to the next character in dest after c, or NULL if c was not found in the first n characters of src.
## ft_memmove
`void	*ft_memmove(void *dest, const void *src, size_t n)`

Copies n bytes from memory area src to memory area dest. The memory areas may overlap.
### Return Value
Returns a pointer to dest.
## ft_memchr
`void *ft_memchr(const void *str, int c, size_t n)`

Scans the initial n bytes of the memory area pointed to by str for the first instance of c. Both c and the bytes of the memory area pointed to by str are interpreted as unsigned char.
### Return Value
Returns a pointer to the matching byte or NULL if the character does not occur in the given memory area.
## ft_memcmp
`int ft_memcmp(const void *buf1, const void *buf2, size_t n)`

Compares the first n bytes (each interpreted as unsigned char) of the memory areas buf1 and buf2.
### Return Value
Returns an integer less than, equal to, or greater than zero if the first n bytes of buf1 is found, respectively, to be less than, to match, or be greater than the first n bytes of buf2.
For a nonzero return value, the sign is determined by the sign of the difference between the first pair of bytes (interpreted as unsigned char) that differ in buf1 and buf2.
## ft_strlen
`size_t	ft_strlen(const char *str)`

Calculates the length of the string str, excluding the terminating null byte.
### Return Value
Returns the number of bytes in the string str.
## ft_strdup
Returns a pointer to a new string which is a duplicate of the string s. Memory for the new string is obtained with **malloc**, and can be freed with **free**.
### Return Value
Returns a pointer to the duplicated string, or NULL if insufficient memory was available.
