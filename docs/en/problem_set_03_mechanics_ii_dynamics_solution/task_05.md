## Problem 5 – Momentum and one-dimensional head-on collision

### Given

Two bodies with masses $m_1$ and $m_2$ move along one straight line.  
The collision is elastic.

Let the initial velocities be $u_1$ and $u_2$, and the final velocities be $v_1$ and $v_2$.

We need to:

- write the principles of conservation of momentum and energy,
- determine the velocities after the collision,
- consider the case $m_1 = m_2$,
- consider the limit $m_2 \gg m_1$,
- interpret the results physically.

---

## 1. Conservation laws

For a one-dimensional elastic collision, two quantities are conserved.

### Conservation of momentum

$$
m_1u_1 + m_2u_2 = m_1v_1 + m_2v_2
$$

### Conservation of kinetic energy

$$
\frac{1}{2}m_1u_1^2 + \frac{1}{2}m_2u_2^2
=
\frac{1}{2}m_1v_1^2 + \frac{1}{2}m_2v_2^2
$$

These two equations are sufficient to determine the final velocities.

---

## 2. Velocities after the collision

For an elastic collision in one dimension, the standard final velocities are

$$
\boxed{
v_1 =
\frac{m_1-m_2}{m_1+m_2}u_1
+
\frac{2m_2}{m_1+m_2}u_2
}
$$

$$
\boxed{
v_2 =
\frac{2m_1}{m_1+m_2}u_1
+
\frac{m_2-m_1}{m_1+m_2}u_2
}
$$

These formulas follow from solving the momentum and energy equations together.

---

## 3. Derivation using relative velocity

A convenient property of a one-dimensional elastic collision is that the relative velocity changes sign:

$$
u_1-u_2 = -(v_1-v_2)
$$

or equivalently,

$$
u_1-u_2 = v_2-v_1
$$

Together with momentum conservation,

$$
m_1u_1 + m_2u_2 = m_1v_1 + m_2v_2
$$

we solve for $v_1$ and $v_2$.

From the relative velocity relation,

$$
v_2 = v_1 + u_1 - u_2
$$

Substitute this into the momentum equation:

$$
m_1u_1 + m_2u_2
=
m_1v_1 + m_2(v_1 + u_1 - u_2)
$$

Expand the right-hand side:

$$
m_1u_1 + m_2u_2
=
(m_1+m_2)v_1 + m_2u_1 - m_2u_2
$$

Move the remaining terms to the left:

$$
m_1u_1 - m_2u_1 + m_2u_2 + m_2u_2
=
(m_1+m_2)v_1
$$

So,

$$
(m_1-m_2)u_1 + 2m_2u_2 = (m_1+m_2)v_1
$$

Hence,

$$
\boxed{
v_1 =
\frac{m_1-m_2}{m_1+m_2}u_1
+
\frac{2m_2}{m_1+m_2}u_2
}
$$

Now use

$$
v_2 = v_1 + u_1 - u_2
$$

Substitute the expression for $v_1$:

$$
v_2
=
\frac{m_1-m_2}{m_1+m_2}u_1
+
\frac{2m_2}{m_1+m_2}u_2
+
u_1-u_2
$$

Bring everything over the common denominator $m_1+m_2$:

$$
v_2
=
\frac{(m_1-m_2)u_1 + 2m_2u_2 + (m_1+m_2)u_1 - (m_1+m_2)u_2}{m_1+m_2}
$$

Group the coefficients:

$$
v_2
=
\frac{2m_1u_1 + (m_2-m_1)u_2}{m_1+m_2}
$$

Thus,

$$
\boxed{
v_2 =
\frac{2m_1}{m_1+m_2}u_1
+
\frac{m_2-m_1}{m_1+m_2}u_2
}
$$

---

## 4. Special case: $m_1 = m_2$

Let

$$
m_1 = m_2 = m
$$

Then the formulas simplify.

For $v_1$:

$$
v_1
=
\frac{m-m}{2m}u_1
+
\frac{2m}{2m}u_2
=
u_2
$$

For $v_2$:

$$
v_2
=
\frac{2m}{2m}u_1
+
\frac{m-m}{2m}u_2
=
u_1
$$

Therefore, when the masses are equal, the bodies exchange velocities:

$$
\boxed{v_1=u_2,\qquad v_2=u_1}
$$

This is a well-known result for elastic head-on collisions.

---

## 5. Limit case: $m_2 \gg m_1$

Now consider the case where the second mass is much larger than the first one.

### Velocity of the first body

Using

$$
v_1 =
\frac{m_1-m_2}{m_1+m_2}u_1
+
\frac{2m_2}{m_1+m_2}u_2
$$

if $m_2 \gg m_1$, then

$$
\frac{m_1-m_2}{m_1+m_2}\approx -1,
\qquad
\frac{2m_2}{m_1+m_2}\approx 2
$$

So,

$$
v_1 \approx -u_1 + 2u_2
$$

### Velocity of the second body

Using

$$
v_2 =
\frac{2m_1}{m_1+m_2}u_1
+
\frac{m_2-m_1}{m_1+m_2}u_2
$$

if $m_2 \gg m_1$, then

$$
\frac{2m_1}{m_1+m_2}\approx 0,
\qquad
\frac{m_2-m_1}{m_1+m_2}\approx 1
$$

Hence,

$$
v_2 \approx u_2
$$

So in this limit,

$$
\boxed{v_1 \approx -u_1 + 2u_2,\qquad v_2 \approx u_2}
$$

A particularly important special case is when the heavy body is initially at rest, that is,

$$
u_2 = 0
$$

Then

$$
v_1 \approx -u_1,
\qquad
v_2 \approx 0
$$

So the light body rebounds with nearly the same speed, while the heavy body remains almost unchanged.

---

## 6. Physical interpretation

The results have clear physical meaning.

- In any elastic collision, both momentum and kinetic energy are conserved.
- If the masses are equal, the bodies simply exchange velocities.
- If one body is much heavier than the other, the heavy body is hardly affected.
- A light body colliding elastically with a very heavy body behaves almost like a ball bouncing from a wall.

Thus, the formulas agree with physical intuition.

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
v_1 =
\frac{m_1-m_2}{m_1+m_2}u_1
+
\frac{2m_2}{m_1+m_2}u_2
}
$$

$$
\boxed{
v_2 =
\frac{2m_1}{m_1+m_2}u_1
+
\frac{m_2-m_1}{m_1+m_2}u_2
}
$$

For equal masses:

$$
\boxed{v_1=u_2,\qquad v_2=u_1}
$$

For $m_2\gg m_1$:

$$
\boxed{v_1\approx -u_1+2u_2,\qquad v_2\approx u_2}
$$
