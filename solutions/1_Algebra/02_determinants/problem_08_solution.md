# Exercise 8. Determinant of a Product

## Problem

Let $A,B$ be square matrices such that $\det A=3$ and $\det B=-5$. Compute $\det(AB)$, $\det(BA)$ and, if it exists, $\det(A^{-1}B)$. Explain why the first two results are equal even though usually $AB\neq BA$.

## Solution

**Method.** For square matrices of the same size

$$
\det(AB)=\det A\cdot\det B,\qquad \det(A^{-1})=\frac{1}{\det A}
$$

**Computation.**

$$
\det(AB)=3\cdot(-5)=-15,\qquad \det(BA)=(-5)\cdot3=-15
$$

The inverse $A^{-1}$ exists because $\det A=3\neq0$, so

$$
\det(A^{-1}B)=\frac{1}{3}\cdot(-5)=-\frac{5}{3}
$$

**Why the first two results are equal.** The matrices $AB$ and $BA$ are usually different, but their determinants are products of the same two numbers, $\det A$ and $\det B$. Multiplication of numbers is commutative, so both give $-15$.

**Verification.** For

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 3 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 0 \\
1 & -5 \\
\end{pmatrix}
$$

with $\det A=3$ and $\det B=-5$:

$$
AB=
\begin{pmatrix}
2 & -5 \\
3 & -15 \\
\end{pmatrix},\qquad BA=
\begin{pmatrix}
1 & 1 \\
1 & -14 \\
\end{pmatrix}
$$

The products are different matrices, but $\det(AB)=-30+15=-15$ and $\det(BA)=-14-1=-15$.
