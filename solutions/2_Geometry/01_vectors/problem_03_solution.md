# Exercise 3. Vector Normalization

## Problem

For $v=(3,4)$ find a unit vector $e$ with the same direction and orientation. Check that $\lVert e\rVert=1$, reconstruct $v$ in the form $v=\lVert v\rVert e$, and explain what changes during normalization and what remains unchanged.

## Solution

**Length of v.**

$$
\lVert v\rVert=\sqrt{3^2+4^2}=\sqrt{25}=5
$$

**Unit vector.** Divide $v$ by its length:

$$
e=\frac{v}{\lVert v\rVert}=\left(\frac35,\ \frac45\right)
$$

**Check.**

$$
\lVert e\rVert=\sqrt{\frac{9}{25}+\frac{16}{25}}=\sqrt{1}=1,\qquad \lVert v\rVert\,e=5\left(\frac35,\ \frac45\right)=(3,\ 4)=v
$$

**What changes and what stays.** Only the length changes, from $5$ to $1$. Because we divide by a positive number, the direction and the orientation stay the same: $e$ points exactly where $v$ points. Dividing by a negative number would reverse the orientation.
