# Exercise 15. Classifying Three Systems

## Problem

For each of the following systems, perform only as much elimination as necessary to recognize its type:

**System 1**

$$
\begin{cases}
x+y=2, \\
x-y=0,
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x+2y=4,
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2, \\
2x+2y=5.
\end{cases}
$$

For each, justify the classification: one solution, infinitely many solutions, or no solution.

## Solution

**System 1.** $R_2\leftarrow R_2-R_1$ gives $-2y=-2$. The remaining equation still contains $y$ with a nonzero coefficient, so there is exactly one solution: $y=1$ and $x=1$.

**System 2.** $R_2\leftarrow R_2-2R_1$ gives $0=0$. The second equation is a multiple of the first, so only one condition remains and there are infinitely many solutions, $(x,\ y)=(2-s,\ s)$ for every real $s$.

**System 3.** $R_2\leftarrow R_2-2R_1$ gives $0=1$, a contradiction. There is no solution.

**Classification.**

| System | Row after one step | Type | Geometry |
|---|---|---|---|
| 1 | $-2y=-2$ | exactly one solution | two lines crossing at one point |
| 2 | $0=0$ | infinitely many solutions | the same line twice |
| 3 | $0=1$ | no solution | two parallel lines |

In each case one elimination step was enough, because the last row already shows the type.

**Check for System 1.** $1+1=2$ and $1-1=0$.
