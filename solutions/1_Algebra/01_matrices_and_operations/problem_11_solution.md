# Exercise 11. When Do Matrices Commute?

## Problem

Given

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}.
$$

Find the conditions on $a,b,c,d$ under which $AB=BA$. Describe the general form of all such matrices $B$.

## Solution

**Method.** Compute both products and compare them entry by entry.

$$
AB=
\begin{pmatrix}
a+c & b+d \\
c & d \\
\end{pmatrix},\qquad BA=
\begin{pmatrix}
a & a+b \\
c & c+d \\
\end{pmatrix}
$$

**Conditions.** Equal entries in each position give

$$
\begin{aligned}
a+c=a &\quad\Rightarrow\quad c=0, \\
b+d=a+b &\quad\Rightarrow\quad d=a, \\
d=c+d &\quad\Rightarrow\quad c=0,
\end{aligned}
$$

and the lower-left entries $c=c$ give no condition.

**Result.** $AB=BA$ exactly when $c=0$ and $d=a$, while $a$ and $b$ are arbitrary:

$$
B=
\begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix}=aI+bN,\qquad N=
\begin{pmatrix}
0 & 1 \\
0 & 0 \\
\end{pmatrix}
$$

**Explanation.** $A=I+N$ itself has this form. Both $I$ and $N$ commute with $A$, so every combination $aI+bN$ does as well, and the computation shows that no other matrix does.

**Verification.** For $a=2$, $b=5$:

$$
A
\begin{pmatrix}
2 & 5 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 7 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 5 \\
0 & 2 \\
\end{pmatrix}A
$$
