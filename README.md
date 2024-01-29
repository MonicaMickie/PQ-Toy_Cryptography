## Overview
This repository contains C code implementing a toy encryption scheme.
The code is organized into functions that perform various operations such as polynomial multiplication, matrix-vector multiplication, encryption, and decryption.

## Code Structure:
### `toy.h`
Header file containing function prototypes, constants, and macro definitions used in the TOY code.
### `toy.c`
Implementation file containing the main TOY encryption and decryption functions.
### `main.c`
Example usage of the TOY encryption and decryption functions.

## Constants and Macros:
- `TK_Q`: Constant representing a prime number used in the TOY encryption scheme.
- `TK_K`: Number of rows in the matrix used in encryption and decryption.
- `TK_N`: Number of columns in the matrix used in encryption and decryption.
- `NEG(X)`: Macro for calculating the negation of a value in the TOY encryption scheme.

## Functions
### `toy_fill_small`
Fills an array with random values following a small Binomial distribution using Hamming weight.
### `toy_polmul_naive`
Performs polynomial multiplication naively, with modulo operations and negations as required by the TOY scheme.
### `toy_mulmv`
Performs matrix-vector multiplication for the TOY encryption scheme.
### `toy_mulmTv`
Performs a variation of matrix-vector multiplication for the TOY encryption scheme.
### `toy_dot`
Calculates the dot product of two vectors with modulo operations and negations as required by the TOY scheme.
### `toy_add`
Adds two vectors with modulo operations and negations as required by the TOY scheme.
### `toy_gen`
Generates random matrices and vectors and performs operations to create an encrypted message for testing purposes.
### `toy_enc`
Encrypts a message using the TOY scheme.
### `toy_dec`
Decrypts a message using the TOY scheme and returns the decrypted plaintext.

## Usage
To use the TOY encryption and decryption functions, include the `toy.h` header file in your code and link it with the implementation file `toy.c`.
Example usage is provided in the `main.c` file.

## Compilation
To compile the code, use a C compiler such as `gcc`
