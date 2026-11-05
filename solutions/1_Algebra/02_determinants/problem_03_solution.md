# Exercise 3. Swapping Two Rows

## Problem

For

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

compute $\det A$. Then form a matrix $B$ by swapping the first and second rows of $A$.

First predict $\det B$ using a determinant property, and then verify your prediction by calculation.

## Solution

**Determinant of A.** Sarrus' rule:

$$
\det A=(1\cdot3\cdot1+2\cdot1\cdot2+0\cdot0\cdot1)-(0\cdot3\cdot2+1\cdot1\cdot1+2\cdot0\cdot1)=7-1=6
$$

**Prediction.** Swapping two rows changes the sign of the determinant, so

$$
\det B=-\det A=-6
$$

**Verification by calculation.**

$$
B=
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

$$
\det B=(0\cdot2\cdot1+3\cdot0\cdot2+1\cdot1\cdot1)-(1\cdot2\cdot2+0\cdot0\cdot1+3\cdot1\cdot1)=1-7=-6
$$

**Result.** $\det A=6$ and $\det B=-6$, so the prediction is confirmed.

**Explanation.** In Sarrus' rule a row swap turns every "plus" product into a "minus" product and vice versa, so every term changes sign and the whole determinant changes sign.
