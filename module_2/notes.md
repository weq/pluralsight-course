# Module 2

## Course Overview

- Data Types
- Variables
- Operators
- Control Flow
  - If/Else
  - Loops
- Ownership and Borrowing
- Functions and Error Handling
- Data Structures
  - Associated methods
- Collections
- Generics
- Concurrency
- Crates and Modules
- Summary

## The Project

The project is called `duckair` and I've placed it in the root of this repo. I created this using `cargo new duckair`.

In Module 2 the tutorial wants us to begin solving the two things mentioned below.

> Create an application that will calculate the great circle route distance between two airports.
>
> Create an application that will calculate the distance between each waypoint along with the total distance.

### Rust Toolchain

#### Channels:

- Stable - 6 week release cycle
- Beta - 6 week release cycle
- Nightly - Nightly release cycle

#### rustup

This is the toolchain management utility.

## Data Storage in Memory

### Stack
This is basically a stack of something, like a stack of plates.
Basically it is "First In, Last Out" (FILO).

### Heap
This is much bigger in size than the stack, and it gets used by having a `ptr` stored in the stack to locate data in the Heap.