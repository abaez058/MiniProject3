MiniProject 3 – Matrix Decomposition Summary

This project performs several matrix decomposition techniques—LU, SVD, and QR—on a given 3×3 matrix, and also computes singular values for a dataset loaded from a JSON file.

Files Used

MiniProject3.py — main script

SVD_dataset.json — dataset used for Question 3

Question 2 – Operations on a 3×3 Matrix
Matrix Used

A fixed 3×3 matrix A2:

[[10, -7,  0],
 [-3,  2,  6],
 [ 5, -1,  5]]

2.1 — LU Decomposition

The script computes:

P (Permutation matrix)

L (Lower triangular with 1s on the diagonal)

U (Upper triangular)

It verifies the result using:

P @ A2 ≈ L @ U

2.2 — Singular Value Decomposition (SVD)

Uses NumPy’s np.linalg.svd() to compute:

U — left singular vectors

Σ — singular values (as a diagonal matrix)

Vᵀ — right singular vectors

Verification:

A2 ≈ U @ Σ @ Vᵀ

2.3 — QR Decomposition

Computes:

Q — orthogonal matrix

R — upper triangular matrix

Checks:

A2 ≈ Q @ R


Also verifies orthogonality:

Qᵀ @ Q ≈ I

Question 3 – SVD on Provided Dataset

Loads a matrix from SVD_dataset.json, then computes singular values using NumPy’s SVD.

Summary

At the end of the script, the program prints:

LU matrices (P, L, U)

Singular values

QR matrices (Q, R)

SVD results for the JSON matrix
