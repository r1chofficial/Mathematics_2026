# Exercise 1. Vector Operations and Their Meaning

## Problem

For $u=(2,-1,3)$ and $v=(-1,4,2)$ compute

$$
u+v,\qquad u-v,\qquad 3u-2v.
$$

Then verify that $(u+v)-v=u$, and explain geometrically what adding two vectors means.

## Solution

**Method.** Vectors are added, subtracted and multiplied by numbers coordinate by coordinate.

$$
\begin{aligned}
u+v &= (2-1,\ -1+4,\ 3+2)=(1,\ 3,\ 5), \\
u-v &= (2+1,\ -1-4,\ 3-2)=(3,\ -5,\ 1), \\
3u-2v &= (6,\ -3,\ 9)-(-2,\ 8,\ 4)=(8,\ -11,\ 5).
\end{aligned}
$$

**Verification.**

$$
(u+v)-v=(1+1,\ 3-4,\ 5-2)=(2,\ -1,\ 3)=u
$$

**Geometric meaning of addition.** Place the start of $v$ at the end of $u$. Then $u+v$ goes from the start of $u$ to the end of $v$: moving by $u$ and then by $v$ is the same as one move by $u+v$. Equivalently, if $u$ and $v$ start at the same point, $u+v$ is the diagonal of the parallelogram they span. Subtracting $v$ undoes the second move, which is why $(u+v)-v=u$.
