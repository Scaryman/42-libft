# 42-libft
School 42 project - Libft
# Table of Contents
* [ft_memset](#ft_memset)
* [ft_bzero](#ft_bzero)
* [ft_memcpy](#ft_memcpy)
* [ft_memccpy](#ft_memccpy)
* [ft_memmove](#ft_memmove)
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
