# MiniProject 3 – Matrix Decomposition Summary

This project performs several matrix decomposition techniques—LU, SVD, and QR—on a given 3×3 matrix, and computes singular values for a dataset loaded from a JSON file.

---

## Files Used
- **MiniProject3.py** — Main script containing all computations  
- **SVD_dataset.json** — Dataset used for Question 3

---

## Question 2 – Operations on a 3×3 Matrix

### Matrix Used
```text
[[10, -7,  0],
 [-3,  2,  6],
 [ 5, -1,  5]]
```

---

## 2.1 — LU Decomposition

The script computes:
- **P** — Permutation matrix  
- **L** — Lower triangular matrix with 1s on the diagonal  
- **U** — Upper triangular matrix  

Verification:
```text
P @ A2 ≈ L @ U
```

---

## 2.2 — Singular Value Decomposition (SVD)

Using NumPy’s `np.linalg.svd()`, the script computes:
- **U** — Left singular vectors  
- **Σ** — Singular values (diagonal matrix)  
- **Vᵀ** — Right singular vectors  

Verification:
```text
A2 ≈ U @ Σ @ Vᵀ
```

---

## 2.3 — QR Decomposition

The script calculates:
- **Q** — Orthogonal matrix  
- **R** — Upper triangular matrix  

Verification:
```text
A2 ≈ Q @ R
```

Orthogonality check:
```text
Qᵀ @ Q ≈ I
```

---

## Question 3 – SVD on Provided Dataset

The script loads a matrix from `SVD_dataset.json` and computes its singular values using NumPy’s SVD function.

---

## Summary of Outputs

The program prints:
- LU decomposition matrices (P, L, U)  
- Singular values for the 3×3 matrix  
- QR decomposition matrices (Q, R)  
- Singular values from the JSON dataset  

---

This project demonstrates the use of NumPy and SciPy for matrix factorizations and numerical verification.
