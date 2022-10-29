# Module 3

## Data Types

Scalar - Holds on value.
Compound - Holds multiple values.

#### Scalar

- Numbers
- Characters and Booleans

#### Compound

- Arrays
- Tuples

#### Strings

---

## Scalar Data Types

### Numbers

Integers are whole numbers and Float are numbers that can have decimal point like `1.2`. If you have a negative value that means it must be a signed value.

#### 8-bit integer

|TypeOfInt|Range|
|--|--|
|u8|0..255|
|i8|-128..127

#### Floating point numbers

Floating point number include fractions of a number, and you only have signed floating points. `f32` & `f64`.

### Characters and Booleans

Boolean, `True` and `False`

Character Byte Size, 4 Bytes which means UNicode-32 table.

---

## Compound Data Types

### Array

Multiple values of a single data type. Arrays are fixed size.

### Tuples

Multiple values, but they can be different data types. Tuples are also fixed size.

---

## String

### String slices (&str)

- Vector of u8 data
- Immutable
- Stored on the heap

You can use it like this `let my_string = "Hello World";`. You can convert a string slice to a String either `String::from("somestring");` 

### Strings (String)

- Vector of u8 data
- Mutable
- Can be stored on the heap, stack or embedded in the compiled code

You can use it like this `let my_string = "Hello World".to_string();`

#### Concatenation

`String` is returned when you concatenate two `&str`.
Two methods for concatenating strings are:

```rust
let duck = "Duck";
let airlines = "Airlines";

// Method 1 - Array concatenation
let airline_name = [duck, " ", airlines].concat();
println!("{}", airline_name);
// returns Duck Airlines

// Method 2 - format!() macro usage.
let airline_name = format!("{} {}", duck, airlines);
println!("{}", airline_name);
// returns Duck Airlines

// Method 3 & 4 - String method push and + style concatention.
let mut slogan = String::new(); // Creates a new empty `string`.
slogan.push_str("We hit the ground"); // Pushes a string into the var.
slogan.push(' '); // Push a single charcter into the variable, and MUST use single-quotes.
slogan = slogan + "every time"; // Classic + style concatenation. NOTE: It must be `&str` on the right side of the `+`.
```
