# Exercise 6. Parameter and Invertibility

## Problem

For

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t \\
\end{pmatrix}
$$

find all values of $t$ for which the matrix is not invertible. Explain how your answer is related to the determinant being zero.

## Solution

**Determinant.**

$$
\det A(t)=t\cdot t-1\cdot2=t^2-2
$$

**Condition.** The matrix is not invertible exactly when its determinant is zero:

$$
t^2-2=0\quad\Leftrightarrow\quad t=\sqrt2\quad\mathrm{or}\quad t=-\sqrt2
$$

**Result.** $A(t)$ is not invertible for $t=\sqrt2$ and $t=-\sqrt2$, and invertible for every other $t$.

**Explanation.** For $t=\sqrt2$ the rows are $(\sqrt2,\ 1)$ and $(2,\ \sqrt2)$, and the second row is $\sqrt2$ times the first. For $t=-\sqrt2$ the second row is $-\sqrt2$ times the first. Dependent rows give determinant zero, and a matrix with dependent rows has no inverse.

**Verification.** $\det A(\sqrt2)=2-2=0$, while for example $\det A(0)=-2\neq0$.
