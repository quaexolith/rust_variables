# rust_variables
Variables in Rust

# Immutablity
Variables are immutable by default. To declare a variable as mutable, the `mut` keyword must be used with the variable's declaration.

# Constants
You aren’t allowed to use mut with constants. Constants aren’t just immutable by default—they’re always immutable. You declare constants using the const keyword instead of the let keyword, and the type of the value must be annotated.

Constants may be set only to a constant expression, not the result of a value that could only be computed at runtime.

```
const THREE_HOURS_IN_SECONDS: u32 = 60 * 60 * 3;
```

# Shadowing
We can shadow a variable by using the same variable’s name and repeating the use of the `let` keyword.

Shadowing is different from marking a variable as `mut`, because we’ll get a compile-time error if we accidentally try to reassign to this variable without using the let keyword. By using let, we can perform a few transformations on a value but have the variable be immutable after those transformations have been completed.

# Boolean Type
As in most other programming languages, a Boolean type in Rust has two possible values: true and false. Booleans are one byte in size. The Boolean type in Rust is specified using bool.

# The Character Type
Rust’s char type is the language’s most primitive alphabetic type.

Note that we specify char literals with single quotes, as opposed to string literals, which use double quotes. Rust’s char type is four bytes in size and represents a Unicode Scalar Value, which means it can represent a lot more than just ASCII. Accented letters; Chinese, Japanese, and Korean characters; emoji; and zero-width spaces are all valid char values in Rust. Unicode Scalar Values range from U+0000 to U+D7FF and U+E000 to U+10FFFF inclusive.
