# Exercise 3. When Can Matrices Be Multiplied?

## Problem

The matrix sizes are

$$
A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}.
$$

For the products

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

## Solution

**Method.** The product $XY$ is defined only if the number of columns of $X$ equals the number of rows of $Y$:

$$
X_{m\times n}\,Y_{n\times p}=(XY)_{m\times p}.
$$

Each entry of $XY$ is a row of $X$ times a column of $Y$, so these two must have the same length.

| Product | Sizes | Inner dimensions | Result |
|---|---|---|---|
| $AB$ | $(2\times3)(3\times4)$ | $3=3$ | $2\times4$ |
| $BA$ | $(3\times4)(2\times3)$ | $4\neq2$ | not defined |
| $BC$ | $(3\times4)(4\times2)$ | $4=4$ | $3\times2$ |
| $CB$ | $(4\times2)(3\times4)$ | $2\neq3$ | not defined |
| $AC$ | $(2\times3)(4\times2)$ | $3\neq4$ | not defined |
| $CA$ | $(4\times2)(2\times3)$ | $2=2$ | $4\times3$ |
| $AD$ | $(2\times3)(2\times2)$ | $3\neq2$ | not defined |
| $DA$ | $(2\times2)(2\times3)$ | $2=2$ | $2\times3$ |

**Result.** Defined: $AB$, $BC$, $CA$, $DA$. Not defined: $BA$, $CB$, $AC$, $AD$.

**Remark.** $AB$ is defined while $BA$ is not, so changing the order of factors can make the product meaningless.
