# Exercise 5. Angle Between Vectors

## Problem

Given $u=(1,1,0)$ and $v=(1,0,1)$:

1. Use the sign of $u\cdot v$ to predict the type of angle.
2. Compute the angle.
3. Compare the result with the prediction.

## Solution

**1. Prediction.** $u\cdot v=1\cdot1+1\cdot0+0\cdot1=1>0$. A positive dot product means the cosine of the angle is positive, so the angle is acute.

**2. The angle.**

$$
\lVert u\rVert=\sqrt{1+1+0}=\sqrt2,\qquad \lVert v\rVert=\sqrt{1+0+1}=\sqrt2
$$

$$
\cos\varphi=\frac{u\cdot v}{\lVert u\rVert\,\lVert v\rVert}=\frac{1}{\sqrt2\cdot\sqrt2}=\frac12\quad\Rightarrow\quad\varphi=60^\circ
$$

**3. Comparison.** The angle $60^\circ$ lies between $0^\circ$ and $90^\circ$, so it is acute, as predicted.

**Remark.** The vectors $u$, $v$ and $u-v=(0,\ 1,\ -1)$ all have length $\sqrt2$, so they form an equilateral triangle, which confirms the angle of $60^\circ$.
