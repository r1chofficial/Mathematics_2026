# Exercise 1. Matrix Size and Entries

## Problem

Given

$$
A=
\begin{pmatrix}
2 & -1 & 3 \\
0 & 4 & 5 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1 \\
\end{pmatrix}.
$$

1. State the sizes of matrices $A$ and $B$.
2. Read off the entries $a_{12}$, $a_{23}$, $b_{21}$, and $b_{32}$.
3. Write the second row of $A$ and the first column of $B$ as vectors.

## Solution

**Method.** A matrix with $m$ rows and $n$ columns has size $m\times n$. In $a_{ij}$ the first index is the row and the second is the column.

**Sizes.** $A$ has 2 rows and 3 columns, $B$ has 3 rows and 2 columns, so $A$ is $2\times3$ and $B$ is $3\times2$.

**Entries.**

$$
a_{12}=-1,\qquad a_{23}=5,\qquad b_{21}=-2,\qquad b_{32}=1.
$$

**Second row of $A$ and first column of $B$.**

$$
r_2(A)=
\begin{pmatrix}
0 & 4 & 5 \\
\end{pmatrix},\qquad c_1(B)=
\begin{pmatrix}
1 \\
-2 \\
4 \\
\end{pmatrix}.
$$

**Verification.** A row of $A$ must have as many components as $A$ has columns (3), and a column of $B$ as many as $B$ has rows (3). Both vectors have 3 components.
