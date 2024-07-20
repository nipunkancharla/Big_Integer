# BigInt C++ Implementation

## Description

This project implements a `BigInt` class in C++ for handling arbitrarily large integers. It provides functionality for basic arithmetic operations, comparisons, and some mathematical functions on integers that exceed the capacity of built-in data types.

## Features

- Basic arithmetic operations: addition, subtraction, multiplication, division, modulo
- Comparison operators
- Increment and decrement operators
- Exponentiation
- Square root calculation
- Special mathematical functions:
  - Nth Catalan number
  - Nth Fibonacci number
  - Factorial

## Class Overview

The `BigInt` class uses a string of digits to represent large integers. It overloads various operators to provide intuitive usage similar to built-in integer types.

## Usage

To use the `BigInt` class in your project:

1. Include the `BigInt` class definition in your C++ file.
2. Create `BigInt` objects using various constructors:

```cpp
BigInt a(123456789);  // From integer
BigInt b("987654321");  // From string
BigInt c(a);  // Copy constructor
```

3. Perform operations:

```cpp
BigInt sum = a + b;
BigInt product = a * b;
BigInt power = a ^ b;  // Exponentiation
```

4. Compare BigInt objects:

```cpp
if (a > b) {
    // Do something
}
```

5. Use mathematical functions:

```cpp
BigInt fib = NthFibonacci(100);
BigInt cat = NthCatalan(50);
BigInt fact = Factorial(30);
```

## Example

The main function in the provided code demonstrates various operations and functions of the `BigInt` class, including:

- Basic arithmetic
- Comparisons
- Incrementation
- Calculating Fibonacci numbers (1 to 100)
- Calculating Catalan numbers (1 to 100)
- Calculating Factorials (1 to 100)

## Compilation and Running

Compile the code using a C++ compiler that supports C++11 or later. For example, using g++:

```
g++ -std=c++11 bigint.cpp -o bigint
./bigint
```

## Notes

- This implementation prioritizes functionality over optimization. For performance-critical applications, further optimizations may be necessary.
- The code uses the `<bits/stdc++.h>` header, which is not standard C++. For portability, consider replacing it with the specific headers needed.

