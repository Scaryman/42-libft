# 42-libft
School 42 project - Libft
# Table of Contents
* [ft_memset](#ft_memset)
## ft_memset
`void	*ft_memset(void *str, int c, size_t n)`

Sets the first n bytes of the block of memory pointed by str to the specified value (interpreted as an unsigned char).
### Parameters
`str` - Pointer to the block of memory to fill.

`c` - Value to be set. The value is passed as an int, but the function fills the block of memory using the unsigned char conversion of this value.

`n` - Number of bytes to be set to the value. size_t is an unsigned integral type.
### Return Value
str is returned.
## ft_bzero
`void	ft_bzero(void *str, size_t n)`

Sets the first n bytes of the block of memory pointed by str to zero.
### Parameters
`str` - Pointer to the block of memory to fill.

`n` - Number of bytes to be set to zero.
### Return Value
None.
