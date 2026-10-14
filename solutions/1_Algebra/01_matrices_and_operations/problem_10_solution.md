# Exercise 10. Columns of a Matrix Product

**1. Products with the columns of $B$.**

$$
Ab_1=A
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix}=
\begin{pmatrix}
1-2+0 \\
0-1+3 \\
\end{pmatrix}=
\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix},\qquad Ab_2=A
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
$$

**2. The full product** $(2\times3)(3\times2)=2\times2$:

$$
AB=
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

**3. Comparison.** The first column of $AB$ is $Ab_1$ and the second column is $Ab_2$.

**Explanation.** Column $j$ of $AB$ is computed as

$$
(AB)_{ij}=\sum_k a_{ik}b_{kj},
$$

which uses only column $b_j$ of $B$. This is exactly the definition of $Ab_j$. Therefore computing $AB$ means applying $A$ to each column of $B$ separately and placing the results side by side.

**Verification.** The columns of $AB$, computed directly, coincide with $Ab_1$ and $Ab_2$ computed separately.
