# Matrix Inversion and Linear Equation Solver

## Overview

This C++ program calculates the inverse of a square matrix \( A \) and solves a system of linear equations using the inverse matrix method. It uses Gaussian elimination for matrix inversion and multiplication to solve \( AX = B \).

## Components Used

- **Matrix A**: Randomly generated square matrix.
- **Matrix B**: Randomly generated column matrix.
- **Matrix C**: Resulting solution matrix \( X \).
- **Matrix inv**: Inverse of matrix \( A \).

## Program Details

### Matrix Generation

- Random square matrix \( A \) and column matrix \( B \) are generated with user-defined dimensions.
- Matrix \( A \) is augmented with the identity matrix to facilitate matrix inversion.

### Gaussian Elimination

- Gaussian elimination is used to transform matrix \( A \) into its reduced row echelon form and simultaneously perform row operations on the augmented identity matrix.

### Inverse Matrix Calculation

- After Gaussian elimination, the augmented part of matrix \( A \) is extracted as the inverse matrix \( inv \).

### Linear Equation Solution

- The program multiplies the inverse matrix \( inv \) with matrix \( B \) to compute matrix \( C \), which represents the solution matrix \( X \).

## Usage

1. **Matrix Dimensions Input**:
   - Enter the number of rows and columns for matrix \( A \).
   - Ensure that \( A \) is a square matrix.

2. **Matrix Initialization**:
   - Random values are generated for matrix \( A \) and \( B \).

3. **Gaussian Elimination**:
   - Performs Gaussian elimination to transform \( A \) and extract its inverse \( inv \).

4. **Matrix Multiplication**:
   - Multiplies \( inv \) with \( B \) to compute \( C \), the solution matrix \( X \).

5. **Output**:
   - Displays the original matrices \( A \) and \( B \), the computed inverse matrix \( inv \), and the resulting solution matrix \( C \).

## Notes

- Ensure proper input validation to handle non-square matrices or invalid dimensions.
- The program assumes the matrices are invertible.
- Adjust the matrix size limits and random number generation range as needed.

