# Exercise 2. Addition and Scalar Multiplication

## Problem

For

$$
A=
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
$$

compute

$$
A+B,\qquad A-B,\qquad 3A-2B.
$$

Explain why matrix addition is possible only for matrices of the same size.

## Solution

**Method.** Addition, subtraction, and multiplication by a scalar are performed entry by entry.

$$
A+B=
\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix},\qquad A-B=
\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}
$$

$$
3A-2B=
\begin{pmatrix}
3-8 & 6+4 \\
-3-0 & 9-10 \\
\end{pmatrix}=
\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}
$$

**Why the sizes must agree.** The sum is defined position by position, so every entry of $A$ needs a partner at the same position in $B$. This is possible only if both matrices have the same number of rows and columns.

**Verification.** The sum and the difference must add up to $2A$:

$$
(A+B)+(A-B)=
\begin{pmatrix}
2 & 4 \\
-2 & 6 \\
\end{pmatrix}=2A.
$$
