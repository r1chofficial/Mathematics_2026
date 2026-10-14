# Exercise 9. Composing Transformations

**Method.** In $RSx=R(Sx)$ the matrix next to the vector acts first. $RSx$ means scale, then rotate. $SRx$ means rotate, then scale.

$$
Sx=
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix},\qquad RSx=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
$$

$$
Rx=
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix},\qquad SRx=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
$$

**Result.** $RSx\neq SRx$.

**Geometric explanation.** $S$ stretches only the horizontal direction. In $RSx$ the original horizontal component is stretched. In $SRx$ the vector is rotated first, so the old vertical component moves to the horizontal axis and that component is stretched instead. A rotation would commute only with a uniform scaling $kI$.

**Verification.** A rotation preserves length, so $\lVert RSx\rVert=\lVert Sx\rVert=\sqrt{8}$, while $\lVert SRx\rVert=\sqrt{17}$. The two results differ even in length.
