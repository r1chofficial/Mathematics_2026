# Exercise 5. Row Operations

## Problem

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

## Solution

**Method.** Adding a multiple of one row to another row does not change the determinant. Swapping two rows would change the sign, and multiplying a row by $k$ would multiply the determinant by $k$. The goal is a triangular matrix.

**Step 1.** $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3+R_1$, determinant unchanged:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5 \\
\end{pmatrix}
$$

**Step 2.** $R_3\leftarrow R_3+2R_2$, determinant unchanged:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7 \\
\end{pmatrix}
$$

**Step 3.** The matrix is triangular, so the determinant is the product of the diagonal entries:

$$
\det A=1\cdot(-3)\cdot(-7)=21
$$

| Operation | Effect on the determinant |
|---|---|
| $R_2\leftarrow R_2-2R_1$ | unchanged |
| $R_3\leftarrow R_3+R_1$ | unchanged |
| $R_3\leftarrow R_3+2R_2$ | unchanged |

**Verification.** Sarrus' rule applied directly to $A$:

$$
\det A=(2+0+24)-(-3+0+8)=26-5=21
$$
