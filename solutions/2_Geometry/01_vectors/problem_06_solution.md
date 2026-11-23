# Exercise 6. Projection and Perpendicular Component

## Problem

Find the projection of $u=(4,2)$ onto the direction $v=(1,1)$. Then compute

$$
r=u-\mathrm{proj}_v\,u
$$

and verify that $r\cdot v=0$. Explain this result geometrically.

## Solution

**Formula.** The projection of $u$ onto the direction of $v$ is

$$
\mathrm{proj}_v\,u=\frac{u\cdot v}{v\cdot v}\,v
$$

**Computation.** $u\cdot v=4+2=6$ and $v\cdot v=1+1=2$, so

$$
\mathrm{proj}_v\,u=\frac62\,(1,\ 1)=(3,\ 3),\qquad r=u-\mathrm{proj}_v\,u=(4,\ 2)-(3,\ 3)=(1,\ -1)
$$

**Verification.**

$$
r\cdot v=1\cdot1+(-1)\cdot1=0,\qquad \mathrm{proj}_v\,u+r=(3,\ 3)+(1,\ -1)=(4,\ 2)=u
$$

**Geometric meaning.** The vector $u$ is split into two parts: $(3,\ 3)$ along the line of $v$, and $r=(1,\ -1)$ perpendicular to it. The projection is like the shadow of $u$ on that line when light falls perpendicularly onto it. The remainder $r$ is the shortest path from the tip of $u$ to the line, and the shortest connection to a line is always perpendicular to it, which is why $r\cdot v=0$.
