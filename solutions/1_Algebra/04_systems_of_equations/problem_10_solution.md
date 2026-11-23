# Exercise 10. A Polynomial Through Three Points

## Problem

Find a polynomial $p(x)=ax^2+bx+c$ whose graph passes through $(0,1)$, $(1,3)$, and $(2,9)$. Reduce the problem to a system of equations and check the result by substituting all three points.

## Solution

**Setting up the system.** The unknowns are the coefficients $a$, $b$, $c$. Each point on the graph gives one equation:

$$
\begin{aligned}
p(0)=1 &\quad\Rightarrow\quad c=1, \\
p(1)=3 &\quad\Rightarrow\quad a+b+c=3, \\
p(2)=9 &\quad\Rightarrow\quad 4a+2b+c=9.
\end{aligned}
$$

**Solving.** With $c=1$ the other two equations become $a+b=2$ and $4a+2b=8$, that is $2a+b=4$. Subtracting $a+b=2$ gives $a=2$, and then $b=0$.

$$
p(x)=2x^2+1
$$

**Check.**

$$
p(0)=1,\qquad p(1)=2+1=3,\qquad p(2)=8+1=9.
$$

All three points lie on the graph.
