# Exercise 15. Associativity of Multiplication and Different Calculation Paths

## Problem

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\quad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix},\quad C=
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

## Solution

**Path 1.** First $AB$, then multiply by $C$:

$$
AB=
\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix},\qquad (AB)C=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}
$$

**Path 2.** First $BC$, then multiply $A$ by it:

$$
BC=
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix},\qquad A(BC)=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}
$$

**Result.** Both paths give the same matrix.

**Number of operations.** Multiplying an $m\times n$ matrix by an $n\times p$ matrix takes $mnp$ multiplications.

| Path | First product | Second product | Multiplications |
|---|---|---|---|
| first $AB$ | $2\cdot3\cdot2=12$ | $2\cdot2\cdot2=8$ | $20$ |
| first $BC$ | $3\cdot2\cdot2=12$ | $2\cdot3\cdot2=12$ | $24$ |

Path 1 is shorter because its intermediate result $AB$ is only $2\times2$, while $BC$ is $3\times2$.

**Explanation.** Associativity means that the brackets may be placed anywhere: the result does not depend on which product is computed first, only the amount of work does. The order of the factors $A$, $B$, $C$ must still stay the same.
