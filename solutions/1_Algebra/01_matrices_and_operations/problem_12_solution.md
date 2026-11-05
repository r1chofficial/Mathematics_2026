# Exercise 12. Formula for a Matrix Power

## Problem

Let

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n+1$.

## Solution

**Powers.**

$$
A^2=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad A^3=
\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix},\qquad A^4=
\begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}
$$

**Conjecture.** Each multiplication by $A$ adds $1$ to the upper-right entry and leaves the other entries unchanged:

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
$$

**Induction step.** Assume the formula holds for $n$. Then

$$
A^{n+1}=A^nA=
\begin{pmatrix}
1\cdot1+n\cdot0 & 1\cdot1+n\cdot1 \\
0\cdot1+1\cdot0 & 0\cdot1+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & n+1 \\
0 & 1 \\
\end{pmatrix},
$$

which is exactly the formula for $n+1$. The formula holds for $n=1$, so it holds for every $n\ge1$.

**Verification.** For $n=2,3,4$ the formula reproduces the matrices computed above.
