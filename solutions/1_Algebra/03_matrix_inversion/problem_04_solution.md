# Exercise 4. Gauss–Jordan

## Problem

Find $A^{-1}$ using the Gauss–Jordan method for

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}.
$$

Show the augmented matrix $[A\mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.

## Solution

**Start.** Write $A$ and $I$ side by side:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$

**Step 1.** $R_2\leftarrow R_2-3R_1$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$

**Step 2.** $R_2\leftarrow -R_2$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

**Step 3.** $R_1\leftarrow R_1-2R_2$:

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

**Result.**

$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}
$$

**Why this works.** Every row operation is the same as multiplying from the left by an invertible matrix. If all the operations together correspond to a matrix $E$, then the left half becomes $EA$ and the right half becomes $EI=E$. When the left half is $I$, we have $EA=I$, so $E=A^{-1}$, and $E$ is exactly what stands on the right.

**Verification.**

$$
AA^{-1}=
\begin{pmatrix}
1\cdot(-5)+2\cdot3 & 1\cdot2+2\cdot(-1) \\
3\cdot(-5)+5\cdot3 & 3\cdot2+5\cdot(-1) \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$
