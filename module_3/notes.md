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
