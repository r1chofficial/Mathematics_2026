# Exercise 5. Row Echelon Form and Number of Solutions

## Problem

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

## Solution

**Reading the matrix.** The matrix is already in row echelon form. It describes the system

$$
\begin{cases}
x+2y-z=3, \\
y+2z=1, \\
0=0.
\end{cases}
$$

**Number of solutions.** The last row is $0=0$, so there is no contradiction and the system is consistent. The columns of $x$ and $y$ contain pivots, the column of $z$ does not. The number of free variables is the number of unknowns minus the number of pivots, $3-2=1$. One free variable means infinitely many solutions.

**Parametric form.** Let $z=t$. Back substitution gives

$$
\begin{aligned}
y &= 1-2t, \\
x &= 3-2y+z=3-2(1-2t)+t=1+5t,
\end{aligned}
$$

so

$$
(x,\ y,\ z)=(1+5t,\ 1-2t,\ t),\qquad t\in\mathbb{R}.
$$

**Why exactly one variable is free.** Each nonzero row fixes its pivot variable in terms of the variables to its right. The column without a pivot is not fixed by any row, so its value can be chosen freely, and every choice gives a solution.

**Check for t = 1.** The point $(6,\ -1,\ 1)$ gives $6-2-1=3$ and $-1+2=1$.
