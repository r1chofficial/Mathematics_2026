# Exercise 13. A Recurrence Written in Matrix Form

## Problem

Let

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence

$$
0,1,1,2,3,5,8,\ldots
$$

and describe the relationship you observe. Then compute

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}
$$

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

## Solution

**Powers.**

$$
F^2=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},\quad F^3=
\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix},\quad F^4=
\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix},\quad F^5=
\begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}
$$

**Relationship.** All entries are terms of the sequence $f_0=0$, $f_1=1$, $f_{k+1}=f_k+f_{k-1}$, that is $0,1,1,2,3,5,8,\ldots$. The pattern is

$$
F^n=
\begin{pmatrix}
f_{n+1} & f_n \\
f_n & f_{n-1} \\
\end{pmatrix}
$$

For example, $F^5$ contains $f_6=8$, $f_5=5$ and $f_4=3$.

**One recurrence step.**

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}=
\begin{pmatrix}
a+b \\
a \\
\end{pmatrix}
$$

The first entry is the sum of the two consecutive terms. The second entry keeps $a$, which becomes the older term in the next step. Starting from $f_1=1$ and $f_0=0$:

$$
\begin{pmatrix}
1 \\
0 \\
\end{pmatrix}\to
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}\to
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}\to
\begin{pmatrix}
3 \\
2 \\
\end{pmatrix}\to
\begin{pmatrix}
5 \\
3 \\
\end{pmatrix}\to\cdots
$$

**Verification.** $F^5=F^4F$ has first row $5+3=8$ and $5$, in agreement with the sequence.
