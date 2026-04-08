## Problem 5 – Momentum and one-dimensional head-on collision

### Problem statement

Two bodies with masses $m_1$ and $m_2$ move along the same straight line.  
Their initial velocities are $u_1$ and $u_2$.  
After the collision, their velocities become $v_1$ and $v_2$.

Assume that the collision is perfectly elastic.

Determine:

- the conservation laws for the collision,
- the final velocities $v_1$ and $v_2$,
- the special case $m_1 = m_2$,
- the limit case $m_2 \gg m_1$,
- the physical interpretation of the result.

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
\frac{1}{2}m_1u_1^2 + \frac{1}{2}m_2u_2^2 = \frac{1}{2}m_1v_1^2 + \frac{1}{2}m_2v_2^2
$$

For an elastic collision, the relative speed of approach is equal to the relative speed of separation:

$$
u_1 - u_2 = -(v_1 - v_2)
$$

This can be rewritten as

$$
u_1 - u_2 = v_2 - v_1
$$

So,

$$
v_2 = v_1 + u_1 - u_2
$$

---

### 2. Final velocity of the first body

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

Rearrange the terms:

$$
m_1u_1 + m_2u_2 - m_2u_1 + m_2u_2 = (m_1 + m_2)v_1
$$

Thus,

$$
(m_1 - m_2)u_1 + 2m_2u_2 = (m_1 + m_2)v_1
$$

Therefore,

$$
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
$$

---

### 3. Final velocity of the second body

Use

$$
v_2 = v_1 + u_1 - u_2
$$

Substitute the expression for $v_1$:

$$
v_2 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2} + u_1 - u_2
$$

Write everything over the common denominator $m_1 + m_2$:

$$
v_2 = \frac{(m_1 - m_2)u_1 + 2m_2u_2 + (m_1 + m_2)u_1 - (m_1 + m_2)u_2}{m_1 + m_2}
$$

Now simplify the numerator:

$$
(m_1 - m_2)u_1 + (m_1 + m_2)u_1 = 2m_1u_1
$$

$$
2m_2u_2 - (m_1 + m_2)u_2 = (m_2 - m_1)u_2
$$

So,

$$
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
$$

Hence, the final velocities are

$$
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
$$

$$
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
$$

---

### 4. Special case: $m_1 = m_2$

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

Therefore, when the masses are equal, the bodies exchange velocities:

$$
v_1 = u_2
$$

$$
v_2 = u_1
$$

---

### 5. Limit case: $m_2 \gg m_1$

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

if $m_2 \gg m_1$, then approximately

$$
v_2 \approx u_2
$$

So, in this limit,

$$
v_1 \approx -u_1 + 2u_2
$$

$$
v_2 \approx u_2
$$

If the heavy body is initially at rest, then

$$
u_2 = 0
$$

and therefore

$$
v_1 \approx -u_1
$$

$$
v_2 \approx 0
$$

So the light body rebounds with almost the same speed, while the heavy body remains almost unchanged.

---

### 6. Physical interpretation

The result has a clear physical meaning:

- in an elastic collision, both momentum and kinetic energy are conserved,
- if the masses are equal, the bodies exchange velocities,
- if one body is much heavier than the other, its velocity changes very little,
- a light body colliding with a very heavy body behaves almost like a ball bouncing from a rigid wall.

---

## Conclusion

The final velocities in a one-dimensional elastic collision are

$$
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
$$

$$
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
$$

For equal masses,

$$
v_1 = u_2
$$

$$
v_2 = u_1
$$

For the limit case $m_2 \gg m_1$,

$$
v_1 \approx -u_1 + 2u_2
$$

$$
v_2 \approx u_2
$$

These results agree with the physical behavior of elastic head-on collisions.
