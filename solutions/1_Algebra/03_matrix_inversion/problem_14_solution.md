# Exercise 14. A Matrix That Is Its Own Inverse

## Problem

Assume that a square matrix $A$ satisfies

$$
A^2=I.
$$

Show that

$$
A^{-1}=A.
$$

Then give an example of a $2\times2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication.

## Solution

**Proof.** The condition $A^2=I$ means

$$
A\cdot A=I.
$$

So the matrix $B=A$ satisfies $AB=BA=I$, which is exactly the definition of the inverse. The inverse is unique, therefore

$$
A^{-1}=A.
$$

**Example.** The matrix that swaps the two coordinates:

$$
A=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}
$$

It is different from $I$ and from $-I$.

**Verification.**

$$
A^2=
\begin{pmatrix}
0\cdot0+1\cdot1 & 0\cdot1+1\cdot0 \\
1\cdot0+0\cdot1 & 1\cdot1+0\cdot0 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

**Geometric meaning.** $A$ is the reflection in the line $y=x$. Reflecting twice brings every point back, so this transformation undoes itself.
