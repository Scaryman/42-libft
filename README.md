# 42-libft
School 42 project - Libft

## ft_memset
`void	*ft_memset(void *str, int c, size_t n)`

Sets the first num bytes of the block of memory pointed by ptr to the specified value (interpreted as an unsigned char).

### Parameters
`str` - Pointer to the block of memory to fill.

`value` - Value to be set. The value is passed as an int, but the function fills the block of memory using the unsigned char conversion of this value.

`num` - Number of bytes to be set to the value. size_t is an unsigned integral type.

### Return Value
str is returned.
