### Variables

#### Variable Type
- Integer
- Floating Point
- Strings
- Boolean

#### Type Declarations
- Can define an alias for a type. May improve clarity
  - type Celsius float64
  - type IDnum int
- Can declare variable using type alias
  - var temp Celsius
  - var pid IDnum

#### Initializing Variables
- Initialize in the declaration:
  - var x int = 100
  - var x = 100
- Initialize after the declaration:
  - var x int // x = 0
  - x = 100

#### Short variable declaration
- x := 100
- Variable is declared as type of expression on the right hand side
- Can do only inside of a function

#### Pointer
- A pointer is an address to data in memory.
- `&` operator returns the address of a variable/function
- `*` operator returns data at an address (deferencing)

#### New function
- Alternate way to create a variable
- `new()` function creates a variable and returns a pointer to the variable
- Variable is initialized to zero
  - ptr := new(int)
  - *ptr = 3

#### Variable Scope
- Variable accessible from block B[j] if: variable is declared in block B[i], and B[i] >= B[j]

#### Deallocating Memory
- Stack vs. Heap
  - Stack is dedicated to function calls
    - Local variables are stored here
    - Deallocated after function completes
  - Heap is persistent

#### Garbage Collection
- Go is `compiled language` which enables garbage collection

#### Type conversions
- var x int16 = 1
- var y int32 = 2
- x = int32(y)

#### Floating Point
- float32 ~6 digits of precision
- float64 ~15 digits of precision
- Complex numbers represented as two floats: real and imaginary
  - var z complex128 = complex(2,3)

#### Strings
-  ASCII and Unicode
  - ASCII:
    - American Standard Code for Information Exchange
    - Character coding - each character is associated with 8-bit number
      - 'A' = 0x41
  - Unicode is 32-bit character code
    - UTF-8 is variable length
      - 8-bit UTF codes are same as ASCII
- `Code point`: Unicode characters
- `Rune`: a code point in Go
- String is sequence of arbitrary bytes
  - Read only

#### Constants
- Expression whose value is known at compile time.
- Type is inferred from righthand side (boolean, string, number)
- iota:
  - Generate a set of related but distinct constants
  - Like enumerated type in other languages
