# 42-libft
School 42 project - Libft
# Table of Contents
* [ft_memset](#ft_memset)
* [ft_bzero](#ft_bzero)
* [ft_memcpy](#ft_memcpy)
* [ft_memccpy](#ft_memccpy)
* [ft_memmove](#ft_memmove)
* [ft_memchr](#ft_memchr)
* [ft_memcmp](#ft_memcmp)
## ft_memset
`void	*ft_memset(void *str, int c, size_t n)`

Sets the first n bytes of the block of memory pointed by str to the specified value (interpreted as an unsigned char).
### Parameters
`str` - Pointer to the block of memory to fill.

`c` - Value to be set. The value is passed as an int, but the function fills the block of memory using the unsigned char conversion of this value.

`n` - Number of bytes to be set to the value. size_t is an unsigned integral type.
### Return Value
Returns a pointer to str.
## ft_bzero
`void	ft_bzero(void *str, size_t n)`

Sets the first n bytes of the block of memory pointed by str to zero.
### Parameters
`str` - Pointer to the block of memory to fill.

`n` - Number of bytes to be set to zero.
### Return Value
None.
## ft_memcpy
`void	*ft_memcpy(void *dest, const void *src, size_t n)`

Copies n bytes from memory area src to memory area dest. The memory areas must not overlap. Use **[ft_memmove](#ft_memmove)** if the memory areas do overlap.
### Parameters
`dest` - Pointer to the destination block of memory.

`src` - Pointer to the source block of memory.

`n` - Number of bytes to be copied.
### Return Value
Returns a pointer to dest.
## ft_memccpy
`void	*ft_memccpy(void *dest, const void *src, int c, size_t n)`

Copies no more than n bytes from memory area src to memory area dest, stopping when the character c is found. If the memory areas overlap, the results are undefined.
### Parameters
`dest` - Pointer to the destination block of memory.

`src` - Pointer to the source block of memory.

`c` - Stopping character.

`n` - Number of bytes to be copied.
### Return Value
Returns a pointer to the next character in dest after c, or NULL if c was not found in the first n characters of src.
## ft_memmove
`void	*ft_memmove(void *dest, const void *src, size_t n)`

Copies n bytes from memory area src to memory area dest. The memory areas may overlap.
### Parameters
`dest` - Pointer to the destination block of memory.

`src` - Pointer to the source block of memory.

`n` - Number of bytes to be copied.
### Return Value
Returns a pointer to dest.
## ft_memchr
`void *ft_memchr(const void *str, int c, size_t n)`

Scans the initial n bytes of the memory area pointed to by str for the first instance of c. Both c and the bytes of the memory area pointed to by str are interpreted as unsigned char.
### Parameters
`str` - Pointer to the block of memory to find in.

`c` - Character to find.

`n` - Number of bytes to scan.
### Return Value
Returns a pointer to the matching byte or NULL if the character does not occur in the given memory area.
## ft_memcmp
`int ft_memcmp(const void *buf1, const void *buf2, size_t n)`

Compares the first n bytes (each interpreted as unsigned char) of the memory areas buf1 and buf2.
### Parameters
`buf2` - Pointer to the first block of memory.

`buf2` - Pointer to the second block of memory.

`n` - Number of bytes to compare.
### Return Value
Returns an integer less than, equal to, or greater than zero if the first n bytes of buf1 is found, respectively, to be less than, to match, or be greater than the first n bytes of buf2.
For a nonzero return value, the sign is determined by the sign of the difference between the first pair of bytes (interpreted as unsigned char) that differ in buf1 and buf2.
