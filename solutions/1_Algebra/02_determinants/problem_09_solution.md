# Exercise 9. Area and the Determinant

## Problem

The vectors

$$
u=
\begin{pmatrix}
3 \\
1 \\
\end{pmatrix},\qquad v=
\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}
$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

## Solution

**Method.** The area of the parallelogram spanned by two vectors in the plane is the absolute value of the determinant of the matrix whose columns are these vectors.

$$
\det
\begin{pmatrix}
3 & 1 \\
1 & 4 \\
\end{pmatrix}=3\cdot4-1\cdot1=11,\qquad \mathrm{area}=|11|=11
$$

**Reversed order.**

$$
\det
\begin{pmatrix}
1 & 3 \\
4 & 1 \\
\end{pmatrix}=1\cdot1-3\cdot4=-11,\qquad \mathrm{area}=|-11|=11
$$

**Result.** The area is $11$. Reversing the order of the vectors changes the sign of the determinant but not the area.

**Explanation.** Swapping two columns changes the sign of the determinant. The sign describes orientation: it is positive when $v$ lies counterclockwise from $u$, as here, and negative in the opposite order. The parallelogram itself is the same figure, so its area does not change.

**Verification.** The parallelogram fits in a $4\times5$ rectangle. Removing two triangles of area $\frac{3}{2}$, two triangles of area $2$ and two unit squares from the corners leaves

$$
20-3-4-2=11
$$
