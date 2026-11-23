# Exercise 14. A Small Change in the Right-Hand Side

## Problem

Compare the systems

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3
\end{cases}
$$

and

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1.
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

## Solution

**The first two equations.** Adding them gives $3x=3$, so $x=1$, and then $y=2-1=1$. They have the unique common solution $(1,\ 1)$.

**First system.** The third equation $3x=3$ also holds for $x=1$. The system is consistent, with the unique solution $(1,\ 1)$.

**Second system.** The third equation would require $3x=3.1$, but the first two equations already force $x=1$, and $3\cdot1=3\neq3.1$. The system is inconsistent.

**In matrix form.** Write $c$ for the right-hand side of the third equation. The operations $R_2\leftarrow R_2-2R_1$, $R_3\leftarrow R_3-3R_1$ and then $R_3\leftarrow R_3-R_2$ give

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & c-3 \\
\end{pmatrix}
$$

For $c=3$ the last row is $0=0$; for $c=3.1$ it is $0=0.1$, a contradiction.

**Why a small change matters.** There are three equations for only two unknowns. The left side of the third equation is the sum of the other two, since $(x+y)+(2x-y)=3x$, so the system is consistent only if the third right-hand side equals exactly $2+1=3$. Geometrically, three lines pass through one common point only in a special position, and moving one line by a tiny amount destroys that point. The type of the system depends on an exact equality, not on how large the change is.
