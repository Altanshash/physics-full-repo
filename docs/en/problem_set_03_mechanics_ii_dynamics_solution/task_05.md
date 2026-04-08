## Problem 5 – Momentum and one-dimensional head-on collision

### Given

Two bodies with masses $m_1$ and $m_2$ move along one straight line.  
The collision is elastic.

Let the initial velocities be $u_1$ and $u_2$, and the final velocities be $v_1$ and $v_2$.

We need to:

- write the conservation laws,
- determine the velocities after the collision,
- consider the case $m_1 = m_2$,
- consider the limit $m_2 \gg m_1$,
- interpret the result physically.

---

## 1. Conservation laws

In a one-dimensional elastic collision, both momentum and kinetic energy are conserved.

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

---

## 2. Relative velocity relation

For a one-dimensional elastic collision, the relative velocity changes sign:

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

## 3. Final velocity of the first body

Start with momentum conservation:

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

## 4. Final velocity of the second body

Use

$$
v_2 = v_1 + u_1 - u_2
$$

Substitute the expression for $v_1$:

$$
v_2 =
\frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
+ u_1 - u_2
$$

Write everything over the common denominator $m_1 + m_2$:

$$
v_2 =
\frac{(m_1 - m_2)u_1 + 2m_2u_2 + (m_1 + m_2)u_1 - (m_1 + m_2)u_2}{m_1 + m_2}
$$

Now simplify the numerator.

For the $u_1$ terms:

$$
(m_1 - m_2)u_1 + (m_1 + m_2)u_1 = 2m_1u_1
$$

For the $u_2$ terms:

$$
2m_2u_2 - (m_1 + m_2)u_2 = (m_2 - m_1)u_2
$$

So,

$$
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
$$

---

## 5. Final formulas

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

## 6. Case $m_1 = m_2$

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

So for equal masses, the bodies exchange velocities:

$$
\boxed{v_1 = u_2,\qquad v_2 = u_1}
$$

---

## 7. Limit case $m_2 \gg m_1$

From

$$
v_1 = \frac{(m_1 - m_2)u_1 + 2m_2u_2}{m_1 + m_2}
$$

if $m_2 \gg m_1$, then

$$
v_1 \approx -u_1 + 2u_2
$$

From

$$
v_2 = \frac{2m_1u_1 + (m_2 - m_1)u_2}{m_1 + m_2}
$$

if $m_2 \gg m_1$, then

$$
v_2 \approx u_2
$$

Therefore,

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

## 8. Physical interpretation

The result is physically reasonable:

- in an elastic collision, both momentum and kinetic energy are conserved,
- if the masses are equal, the bodies exchange velocities,
- if one body is much heavier, it is barely affected,
- a light body hitting a very heavy body behaves almost like a ball bouncing off a wall.

---

## Final answers

$$
\boxed{
m_1u_1 + m_2u_2 = m_1v_1 + m_2v_2
}
$$

$$
\boxed{
\frac{1}{2}m_1u_1^2 + \frac{1}{2}m_2u_2^2
=
\frac{1}{2}m_1v_1^2 + \frac{1}{2}m_2v_2^2
}
$$

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

$$
\boxed{v_1 = u_2,\qquad v_2 = u_1 \quad \text{if } m_1 = m_2}
$$

$$
\boxed{v_1 \approx -u_1 + 2u_2,\qquad v_2 \approx u_2 \quad \text{if } m_2 \gg m_1}
$$
