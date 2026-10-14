# Exercise 5. Matrix Times Vector

**Row view.** Each entry of $Ax$ is a row of $A$ times $x$:

$$
Ax=
\begin{pmatrix}
2\cdot4+(-1)\cdot2 \\
1\cdot4+3\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

**Column view.** The entries of $x$ are the coefficients of the columns of $A$:

$$
Ax=4
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}+2
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}=
\begin{pmatrix}
8-2 \\
4+6 \\
\end{pmatrix}=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

**Result.** $Ax=(6,\ 10)^T=4a_1+2a_2$, where $a_1,a_2$ are the columns of $A$.

**Explanation.** Both views use the same products, grouped differently. The column view shows that $Ax$ is always a linear combination of the columns of $A$, and $x$ says how much of each column is taken.

**Verification.** The two independent methods give the same vector.
