# Exercise 4. Matrix Multiplication and Noncommutativity

**Method.** Entry $(i,j)$ of a product is row $i$ of the left factor times column $j$ of the right factor.

$$
AB=
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
2\cdot1+0\cdot0 & 2\cdot2+0\cdot1 \\
3\cdot1+1\cdot0 & 3\cdot2+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
$$

**Result.** $AB\neq BA$. Already the upper-left entries differ: $8\neq2$.

**Explanation.** For numbers $ab=ba$, but for matrices this fails in general: $AB$ combines rows of $A$ with columns of $B$, while $BA$ combines rows of $B$ with columns of $A$. This is called noncommutativity, and it means the order of factors must always be kept.

**Verification.** Trace and determinant must be the same for $AB$ and $BA$: $\mathrm{tr}(AB)=\mathrm{tr}(BA)=9$ and $\det(AB)=\det(BA)=2=\det A\cdot\det B$.
