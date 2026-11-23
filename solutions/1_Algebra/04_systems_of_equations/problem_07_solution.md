# Exercise 7. Choosing a Method Deliberately

## Problem

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. one system with a triangular coefficient matrix

$$
\begin{cases}
2x-y=3, \\
4y=8;
\end{cases}
$$

2. three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known;
3. one $3\times3$ system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary. Do not judge a method by its name alone — refer to the number of right-hand sides and the structure of the matrix.

## Solution

**Case 1: triangular matrix, so back substitution.** The coefficient matrix is already triangular, so no elimination is needed. Start from the last equation:

$$
4y=8\quad\Rightarrow\quad y=2,\qquad 2x-2=3\quad\Rightarrow\quad x=\frac52.
$$

Check: $2\cdot\frac52-2=3$ and $4\cdot2=8$.

**Case 2: three right-hand sides with known inverse, so multiplication by the inverse.** Each solution is

$$
x_i=A^{-1}b_i,\qquad i=1,2,3.
$$

The expensive part, the inverse, is already done and is reused three times. Each system then costs only one matrix-vector product, and no elimination is needed at all.

**Case 3: one 3×3 system without a given inverse, so Gaussian elimination.** Plan: write the augmented matrix $[A\mid b]$, create zeros below the diagonal, then use back substitution. Computing $A^{-1}$ here would be unnecessary work: Gauss–Jordan for the inverse carries three extra columns of the identity matrix, which is roughly the work of solving three systems in order to answer one.

**Summary.**

| Situation | Method | Reused or unnecessary |
|---|---|---|
| one system, triangular matrix | back substitution | elimination unnecessary |
| same matrix, three right-hand sides, inverse known | $x_i=A^{-1}b_i$ | inverse reused three times |
| one general system, no inverse | Gaussian elimination | computing the inverse unnecessary |
