# Exercise 9. Matrix Equation

## Problem

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}.
$$

Solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

## Solution

**Which side.** In $AX=B$ the matrix $A$ stands to the left of $X$. Multiplying both sides from the left by $A^{-1}$ gives

$$
A^{-1}AX=A^{-1}B\quad\Rightarrow\quad X=A^{-1}B.
$$

Multiplying from the right would give $AXA^{-1}$, which cannot be simplified, because matrices do not commute.

**Computation.** $\det A=1$, so

$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix},\qquad X=A^{-1}B=
\begin{pmatrix}
3-4 & 1-8 \\
2 & 4 \\
\end{pmatrix}=
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}
$$

**Verification.**

$$
AX=
\begin{pmatrix}
-1+4 & -7+8 \\
2 & 4 \\
\end{pmatrix}=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}=B
$$

**Remark.** The wrong order $BA^{-1}$ gives a different matrix, with first row $3,\ -5$, so the side really matters.
