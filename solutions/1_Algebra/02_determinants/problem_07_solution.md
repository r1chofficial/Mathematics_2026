# Exercise 7. Using Properties Instead of Recomputing

## Problem

Suppose that for a $3\times3$ matrix, $\det A=-4$. Compute

$$
\det(2A),\qquad \det(A^T),\qquad \det(A^2),\qquad \det(-A).
$$

Justify each answer using the appropriate property.

## Solution

For a $3\times3$ matrix with $\det A=-4$:

| Quantity | Property used | Value |
|---|---|---|
| $\det(2A)$ | $\det(kA)=k^n\det A$ with $n=3$ | $2^3\cdot(-4)=-32$ |
| $\det(A^T)$ | $\det(A^T)=\det A$ | $-4$ |
| $\det(A^2)$ | $\det(XY)=\det X\cdot\det Y$ | $(-4)^2=16$ |
| $\det(-A)$ | $\det(kA)=k^n\det A$ with $k=-1$ | $(-1)^3\cdot(-4)=4$ |

**Explanation.**

- $2A$ multiplies each of the three rows by $2$, and each row contributes one factor $2$, hence $2^3=8$.
- Transposing exchanges rows and columns but keeps the determinant.
- $A^2=AA$, so the product rule gives $(\det A)^2$.
- $-A$ multiplies all three rows by $-1$. An odd number of sign changes gives the factor $-1$.

**Verification.** For the diagonal matrix $A=\mathrm{diag}(-4,\ 1,\ 1)$ with $\det A=-4$:

$$
\det(2A)=(-8)\cdot2\cdot2=-32,\qquad \det(A^2)=16\cdot1\cdot1=16,\qquad \det(-A)=4\cdot(-1)\cdot(-1)=4
$$
