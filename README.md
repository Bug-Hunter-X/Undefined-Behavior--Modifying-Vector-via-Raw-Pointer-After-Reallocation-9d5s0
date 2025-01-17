# Rust Undefined Behavior Example

This repository demonstrates a common source of undefined behavior in Rust: modifying a vector's contents through a raw pointer after the vector's capacity has been exceeded.  The code attempts to modify the first element of the vector using a raw pointer, but this leads to undefined behavior if the vector's internal data is reallocated.