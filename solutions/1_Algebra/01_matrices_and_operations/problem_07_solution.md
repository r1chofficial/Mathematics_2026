# Exercise 7. Identity Matrix, Zero Matrix, and Powers

**Neutral elements.** $AI=IA=A$ and $A+0=A$.

- $I$ is the neutral element of multiplication, like $1$ for numbers.
- $0$ is the neutral element of addition, like $0$ for numbers.

**Powers.**

$$
A^2=
\begin{pmatrix}
4+0 & 2+2 \\
0 & 0+4 \\
\end{pmatrix}=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix},\qquad A^3=A^2A=
\begin{pmatrix}
8+0 & 4+8 \\
0 & 0+8 \\
\end{pmatrix}=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
$$

**Pattern.** The diagonal entries are $2,4,8$, i.e. $2^n$. The upper-right entries are $1,4,12$, i.e. $n\,2^{n-1}$. The lower-left entry stays $0$:

$$
A^n=
\begin{pmatrix}
2^n & n\,2^{n-1} \\
0 & 2^n \\
\end{pmatrix}
$$

**Verification.** $\det A=4$, so $\det A^3$ must be $4^3=64$. Indeed $8\cdot8-12\cdot0=64$.
