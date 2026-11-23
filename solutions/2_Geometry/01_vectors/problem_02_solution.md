# Exercise 2. Distance as the Length of a Vector

## Problem

The points are $A=(1,2,3)$ and $B=(4,-2,6)$.

1. Construct $\overrightarrow{AB}$.
2. Compute its length.
3. Compute the distance between the points using the coordinate formula.
4. Explain why both calculations give the same result.

## Solution

**1. The vector.** Subtract the start point from the end point:

$$
\overrightarrow{AB}=B-A=(4-1,\ -2-2,\ 6-3)=(3,\ -4,\ 3)
$$

**2. Its length.**

$$
\lVert\overrightarrow{AB}\rVert=\sqrt{3^2+(-4)^2+3^2}=\sqrt{9+16+9}=\sqrt{34}
$$

**3. The distance formula.**

$$
d(A,B)=\sqrt{(4-1)^2+(-2-2)^2+(6-3)^2}=\sqrt{34}\approx5.83
$$

**4. Why the results agree.** The distance formula takes the differences of the coordinates, squares them and adds them. These differences are exactly the coordinates of $\overrightarrow{AB}$, so the distance formula is just the length of $\overrightarrow{AB}$ written out. Both come from the Pythagorean theorem in three dimensions.
