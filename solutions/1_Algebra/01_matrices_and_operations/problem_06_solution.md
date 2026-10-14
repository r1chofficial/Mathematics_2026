# Exercise 6. Transpose

**Method.** The transpose turns rows into columns. An $m\times n$ matrix becomes $n\times m$:

$$
(A^T)_{ij}=a_{ji}
$$

$$
A^T=
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix},\qquad B^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
1+4-3 & 0+2+9 \\
4+10-6 & 0+5+18 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix},\qquad (AB)^T=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

**Verification of the property.**

$$
B^TA^T=
\begin{pmatrix}
1+4-3 & 4+10-6 \\
0+2+9 & 0+5+18 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}=(AB)^T
$$

**Explanation.** The order of factors must reverse. Keeping the order is impossible here: $A^TB^T$ would be $(3\times2)(2\times3)$, a $3\times3$ matrix, while $(AB)^T$ is $2\times2$.
