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
