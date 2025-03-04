# Eigenvalue Decomposition

# Overview

This notebook consists of the mathematical and computational solution to the problem of verifying whether a given matrix is positive definite, performing its eigendecomposition, and verifying key matrix identities

# Problem Statement

Attached below is the screenshot of the problem statement

![Screenshot 2025-02-28 175900](https://github.com/user-attachments/assets/8ca4f521-d79a-4190-bc1a-f9347af41a8b)

# Methodology

(a) <ins> Checking Positive Definiteness </ins>

A matrix is positive definite if:

1. All its eigenvectors are positive

2. Alternatively, using Sylvestor's criterion, all leading principal minors are positive.

(b) <ins> Eigendecomposition </ins>

We solve for the eigenvalues and eigenvectors by solving:

           det(A - λI) = 0

and computing the corresponding eigenvectors.

(c) <ins> Verification </ins>

1. Compute A^2 directly and verify that it matches Vʌ^2V^T.

2. Compute the inverse A^-1 and verify that it matches Vʌ^-1V^T.

# Implementation

The calculations were performed mathematically and verified using Python. The implementation:

1. Computes eigenvalues and eigenvectors using

             numpy.linalg.eigh

2. Constructs VʌV^T and compares the results numerically.

3. Verifies the positive definiteness using determinant conditions.

# Results

1. The matrix was confirmed to be positive definite.

2. Eigendecomposition successfully provided orthonormal eigenvectors and corresponding eigenvalues.

3. Matrix identities were verified numerically.

# Dependencies

1. Python 3

2. NumPy

3. Pandas

# Conclusion

The problem was successfully solved using both analytical and numerical methods, confirming the matrix's properties and decomposition.
