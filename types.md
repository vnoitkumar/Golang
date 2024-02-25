# Types

## Numeric Types:

- uint: Unsigned integer type,  either 32 or 64 bits
- int: Signed integer type, same size as uint
- int8, int16, int32, int64: Signed integers of specific bit sizes.
- uint8, uint16, uint32, uint64, uintptr: Unsigned integers of specific bit sizes.
- float32, float64: Floating-point types.
- complex64, complex128: Complex number types.
- byte: An alias for uint8, often used to represent ASCII characters.
- rune: An alias for int32, represents a Unicode code point.
- uintptr: An unsigned integer large enough to store the uninterpreted bits of a pointer value

### Detailed explination
### uint 
- uint8       the set of all unsigned  8-bit integers (0 to 255)
- uint16      the set of all unsigned 16-bit integers (0 to 65535)
- uint32      the set of all unsigned 32-bit integers (0 to 4294967295)
- uint64      the set of all unsigned 64-bit integers (0 to 18446744073709551615)

### int
- int8        the set of all signed  8-bit integers (-128 to 127)
- int16       the set of all signed 16-bit integers (-32768 to 32767)
- int32       the set of all signed 32-bit integers (-2147483648 to 2147483647)
- int64       the set of all signed 64-bit integers (-9223372036854775808 to 9223372036854775807)

### float
- float32     the set of all IEEE-754 32-bit floating-point numbers
- float64     the set of all IEEE-754 64-bit floating-point numbers

### complex
- complex64   the set of all complex numbers with float32 real and imaginary parts
- complex128  the set of all complex numbers with float64 real and imaginary parts

### alias
- byte        alias for uint8
- rune        alias for int32

## Boolean Type:
- bool: Represents true/false values.

## String Type:
- string: Represents a sequence of bytes.

## Composite Types:
- array: Represents a fixed-size array of elements.
- slice: Represents a dynamically-sized sequence.
- map: Represents an unordered collection of key-value pairs.
- struct: Represents a collection of fields.

## Pointer Types:
- pointer: Represents the memory address of a value.

## Function Types:
- func: Represents a function.

## Interface Types:
- interface: Specifies a set of methods that a concrete type must implement to be considered an instance of that interface.

## Channel Type:

- chan: Represents a communication channel for Goroutines.

## Error Type:
- error: Represents an error condition.

## Special Types:
- nil: Represents a zero value for pointers, interfaces, channels, and maps.