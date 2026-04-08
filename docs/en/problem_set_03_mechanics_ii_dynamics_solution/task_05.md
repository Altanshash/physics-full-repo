## Problem 5 – Momentum and one-dimensional head-on collision

### Problem statement

Two bodies with masses $m_1$ and $m_2$ move along the same straight line.  
Their initial velocities are $u_1$ and $u_2$.  
After the collision, their velocities become $v_1$ and $v_2$.

Assume that the collision is perfectly elastic.

Determine:

- the conservation laws for the collision,
- the velocities $v_1$ and $v_2$ after the collision,
- the special case when $m_1 = m_2$,
- the limit case when $m_2 \gg m_1$,
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
\frac{1}{2}m_1u_1^2 + \frac{1}{2}m_2u_2^2
=
\frac{1}{2}m_1v_1^2 + \frac{1}{2}m_2v_2^2
$$

For an elastic collision, the relative velocity also changes sign:

$$
u_1 - u_2 = -(v_1 - v_2)
$$

This can be written as

$$
u_1 - u_2 = v_2 - v_1
$$

Hence,

$$
v_2 = v_1 + u_1 - u_2
$$

---

### 2. Finding $v_1$

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

So,

$$
(m_1 - m_2)u_1 + 2m_2u_2 = (m_1 + m_2)v_1
$$

Therefore,

$$
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
$$

---

### 3. Finding $v_2$

Use

$$
v_2 = v_1 + u_1 - u_2
$$

Substitute the expression for $v_1$:

$$
v_2
=
\frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
+ u_1 - u_2
$$

Write everything over the common denominator $m_1 + m_2$:

$$
v_2
=
\frac{(m_1 - m_2)u_1 + 2m_2u_2 + (m_1 + m_2)u_1 - (m_1 + m_2)u_2}{m_1 + m_2}
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

Thus, the final velocities are

$$
\boxed{
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
}
$$

$$
\boxed{
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
}
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

Therefore, if the masses are equal, the two bodies exchange velocities:

$$
\boxed{v_1 = u_2,\qquad v_2 = u_1}
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

if $m_2 \gg m_1$, then

$$
v_2 \approx u_2
$$

So, in this limit,

$$
\boxed{v_1 \approx -u_1 + 2u_2,\qquad v_2 \approx u_2}
$$

A very important special case is when the heavy body is initially at rest:

$$
u_2 = 0
$$

Then

$$
\boxed{v_1 \approx -u_1,\qquad v_2 \approx 0}
$$

---

### 6. Physical interpretation

The result is physically meaningful:

- in an elastic collision, both momentum and kinetic energy are conserved,
- if the masses are equal, the bodies exchange velocities,
- if one body is much heavier, its velocity changes very little,
- a light body hitting a very heavy body behaves almost like a ball bouncing from a rigid wall.

---

## Conclusion

For a one-dimensional elastic collision, the final velocities are

$$
\boxed{
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
}
$$

$$
\boxed{
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
}
$$

If $m_1 = m_2$, the bodies exchange velocities:

$$
\boxed{v_1 = u_2,\qquad v_2 = u_1}
$$

If $m_2 \gg m_1$, then approximately

$$
\boxed{v_1 \approx -u_1 + 2u_2,\qquad v_2 \approx u_2}
$$

These results agree with the physical interpretation of elastic collisions.
