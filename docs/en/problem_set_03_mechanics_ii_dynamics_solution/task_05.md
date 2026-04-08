## Problem 5 – Momentum and one-dimensional head-on collision

### Problem statement

Two bodies with masses $m_1$ and $m_2$ move along the same straight line.  
Their initial velocities are $u_1$ and $u_2$.  
After the collision, their velocities become $v_1$ and $v_2$.

Assume that the collision is perfectly elastic.

Determine:

- the conservation laws,
- the final velocities $v_1$ and $v_2$,
- the case $m_1 = m_2$,
- the limit case $m_2 \gg m_1$,
- the physical meaning of the result.

---

## Solution

### 1. Conservation laws

For a one-dimensional elastic collision, both momentum and kinetic energy are conserved.

Momentum conservation:

$$
m_1u_1 + m_2u_2 = m_1v_1 + m_2v_2
$$

Kinetic energy conservation:

$$
\frac{1}{2}m_1u_1^2 + \frac{1}{2}m_2u_2^2
=
\frac{1}{2}m_1v_1^2 + \frac{1}{2}m_2v_2^2
$$

For an elastic collision, the relative speed of approach is equal to the relative speed of separation:

$$
u_1 - u_2 = -(v_1 - v_2)
$$

So we can write

$$
u_1 - u_2 = v_2 - v_1
$$

and therefore

$$
v_2 = v_1 + u_1 - u_2
$$

---

### 2. Determination of $v_1$

Start from momentum conservation:

$$
m_1u_1 + m_2u_2 = m_1v_1 + m_2v_2
$$

Substitute

$$
v_2 = v_1 + u_1 - u_2
$$

Then

$$
m_1u_1 + m_2u_2 = m_1v_1 + m_2(v_1 + u_1 - u_2)
$$

Expand the right-hand side:

$$
m_1u_1 + m_2u_2 = m_1v_1 + m_2v_1 + m_2u_1 - m_2u_2
$$

Group the terms with $v_1$:

$$
m_1u_1 + m_2u_2 = (m_1 + m_2)v_1 + m_2u_1 - m_2u_2
$$

Move the remaining terms to the left:

$$
m_1u_1 - m_2u_1 + m_2u_2 + m_2u_2 = (m_1 + m_2)v_1
$$

Thus,

$$
(m_1 - m_2)u_1 + 2m_2u_2 = (m_1 + m_2)v_1
$$

Hence,

$$
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
$$

---

### 3. Determination of $v_2$

Use

$$
v_2 = v_1 + u_1 - u_2
$$

Substitute the expression for $v_1$:

$$
v_2 =
\frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2} + u_1 - u_2
$$

Write everything over the common denominator $m_1 + m_2$:

$$
v_2 =
\frac{(m_1 - m_2)u_1 + 2m_2u_2 + (m_1 + m_2)u_1 - (m_1 + m_2)u_2}{m_1 + m_2}
$$

Now simplify the numerator.

For the terms with $u_1$:

$$
(m_1 - m_2)u_1 + (m_1 + m_2)u_1 = 2m_1u_1
$$

For the terms with $u_2$:

$$
2m_2u_2 - (m_1 + m_2)u_2 = (m_2 - m_1)u_2
$$

So,

$$
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
$$

Therefore, the final velocities are

$$
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
$$

$$
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
$$

---

### 4. Case $m_1 = m_2$

Let

$$
m_1 = m_2 = m
$$

Then

$$
v_1 = \frac{(m - m)u_1 + 2mu_2}{2m} = u_2
$$

and

$$
v_2 = \frac{2mu_1 + (m - m)u_2}{2m} = u_1
$$

So, if the masses are equal, the two bodies exchange velocities:

$$
v_1 = u_2
$$

$$
v_2 = u_1
$$

---

### 5. Limit case $m_2 \gg m_1$

From the formula for $v_1$:

$$
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
$$

if $m_2 \gg m_1$, then approximately

$$
v_1 \approx -u_1 + 2u_2
$$

From the formula for $v_2$:

$$
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
$$

if $m_2 \gg m_1$, then

$$
v_2 \approx u_2
$$

Thus,

$$
v_1 \approx -u_1 + 2u_2
$$

$$
v_2 \approx u_2
$$

A particularly important case is when the heavy body is initially at rest:

$$
u_2 = 0
$$

Then

$$
v_1 \approx -u_1
$$

$$
v_2 \approx 0
$$

So the lighter body rebounds with nearly the same speed, while the heavier body remains almost unchanged.

---

### 6. Physical interpretation

The result has a clear physical meaning:

- in an elastic collision, both momentum and kinetic energy are conserved,
- if the masses are equal, the bodies exchange velocities,
- if one body is much heavier than the other, its velocity changes very little,
- a light body colliding with a very heavy body behaves almost like a ball reflecting from a wall.

---

## Conclusion

The final velocities in a one-dimensional elastic collision are

$$
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
$$

$$
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
$$

If $m_1 = m_2$, then the bodies exchange velocities:

$$
v_1 = u_2, \qquad v_2 = u_1
$$

If $m_2 \gg m_1$, then approximately

$$
v_1 \approx -u_1 + 2u_2, \qquad v_2 \approx u_2
$$

These results are fully consistent with the physical behavior of elastic collisions.
