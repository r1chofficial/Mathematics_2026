# Exercise 7. Linear Dependence Without Heavy Computation

## Problem

Given

$$
u=(1,2,3),\qquad v=(2,4,6),\qquad w=(0,1,1).
$$

Identify a specific relation between $u$ and $v$, decide whether the three vectors can be linearly independent, and explain why no long calculation is needed.

## Solution

**Relation between u and v.**

$$
v=(2,\ 4,\ 6)=2\cdot(1,\ 2,\ 3)=2u
$$

**Dependence.** This gives a combination with coefficients that are not all zero and that equals the zero vector:

$$
2u-v+0\cdot w=(0,\ 0,\ 0)
$$

By definition, the vectors $u$, $v$, $w$ are therefore linearly dependent. They cannot be independent, whatever $w$ is.

**Why no long calculation is needed.** A set that contains two parallel vectors is always dependent, because one of them is a multiple of the other, so the third vector does not matter at all. Geometrically, $u$ and $v$ lie on one line, so all three vectors lie in one plane, the plane spanned by $u$ and $w$, and cannot fill three-dimensional space.

**Check.** The determinant of the matrix with rows $u$, $v$, $w$ is $0$, because two of its rows are proportional.
