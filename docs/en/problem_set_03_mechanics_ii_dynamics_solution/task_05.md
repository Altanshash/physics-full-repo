## Problem 5 – Momentum and one-dimensional head-on collision

### Given

Two bodies with masses $m_1$ and $m_2$ move along the same straight line.  
The collision is elastic.

Let the initial velocities be

$$
u_1,\qquad u_2
$$

and the final velocities be

$$
v_1,\qquad v_2.
$$

We need to:

- write the conservation laws,
- determine the velocities after the collision,
- consider the case $m_1=m_2$,
- consider the limit $m_2 \gg m_1$,
- interpret the result physically.

---

## 1. Conservation of momentum and kinetic energy

For a one-dimensional elastic collision, both momentum and kinetic energy are conserved.

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

These two equations determine the final velocities.

---

## 2. Useful relation for an elastic collision

In a one-dimensional elastic collision, the relative speed of approach equals the relative speed of separation:

$$
u_1-u_2 = -(v_1-v_2)
$$

This can also be written as

$$
u_1-u_2 = v_2-v_1
$$

or equivalently

$$
v_1-v_2 = -(u_1-u_2)
$$

We use this relation together with momentum conservation.

---

## 3. Derivation of the final velocities

From the relative velocity relation,

$$
u_1-u_2 = v_2-v_1
$$

so

$$
v_2 = v_1 + u_1 - u_2
$$

Now substitute this into the momentum equation:

$$
m_1u_1 + m_2u_2 = m_1v_1 + m_2(v_1 + u_1 - u_2)
$$

Expand the right-hand side:

$$
m_1u_1 + m_2u_2 = m_1v_1 + m_2v_1 + m_2u_1 - m_2u_2
$$

Collect the terms containing $v_1$:

$$
m_1u_1 + m_2u_2 = (m_1+m_2)v_1 + m_2u_1 - m_2u_2
$$

Move the remaining terms to the left-hand side:

$$
m_1u_1 - m_2u_1 + m_2u_2 + m_2u_2 = (m_1+m_2)v_1
$$

This gives

$$
(m_1-m_2)u_1 + 2m_2u_2 = (m_1+m_2)v_1
$$

Therefore,

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

Write the last two terms over the common denominator $m_1+m_2$:

$$
v_2
=
\frac{(m_1-m_2)u_1 + 2m_2u_2 + (m_1+m_2)u_1 - (m_1+m_2)u_2}{m_1+m_2}
$$

Now simplify the numerator:

- coefficient of $u_1$:

$$
(m_1-m_2)+(m_1+m_2)=2m_1
$$

- coefficient of $u_2$:

$$
2m_2-(m_1+m_2)=m_2-m_1
$$

So,

$$
\boxed{
v_2 =
\frac{2m_1}{m_1+m_2}u_1
+
\frac{m_2-m_1}{m_1+m_2}u_2
}
$$

Thus, the final velocities after the collision are

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

---

## 4. Special case: $m_1 = m_2$

Let

$$
m_1=m_2=m
$$

Substitute into the formula for $v_1$:

$$
v_1
=
\frac{m-m}{2m}u_1 + \frac{2m}{2m}u_2
=
0\cdot u_1 + u_2
=
u_2
$$

Now for $v_2$:

$$
v_2
=
\frac{2m}{2m}u_1 + \frac{m-m}{2m}u_2
=
u_1 + 0\cdot u_2
=
u_1
$$

Therefore, for equal masses the bodies exchange velocities:

$$
\boxed{v_1=u_2,\qquad v_2=u_1}
$$

---

## 5. Limit case: $m_2 \gg m_1$

Now suppose the second body is much heavier than the first one.

### Velocity of the first body

Start from

$$
v_1 =
\frac{m_1-m_2}{m_1+m_2}u_1
+
\frac{2m_2}{m_1+m_2}u_2
$$

If $m_2 \gg m_1$, then

$$
\frac{m_1-m_2}{m_1+m_2}\approx -1,
\qquad
\frac{2m_2}{m_1+m_2}\approx 2
$$

Hence,

$$
\boxed{v_1 \approx -u_1 + 2u_2}
$$

### Velocity of the second body

From

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

So,

$$
\boxed{v_2 \approx u_2}
$$

Thus, in this limit,

$$
\boxed{v_1 \approx -u_1 + 2u_2,\qquad v_2 \approx u_2}
$$

A very important special case is when the heavy body is initially at rest:

$$
u_2 = 0
$$

Then

$$
v_1 \approx -u_1,
\qquad
v_2 \approx 0
$$

So the light body rebounds with almost the same speed, while the heavy body remains almost unchanged.

---

## 6. Physical interpretation

These formulas have a clear physical meaning.

- In any elastic collision, both momentum and kinetic energy are conserved.
- If the masses are equal, the two bodies simply exchange velocities.
- If one mass is much larger than the other, the heavier body is almost unaffected.
- A light body hitting a very heavy body behaves almost like a ball bouncing from a rigid wall.

Therefore, the mathematical result agrees with physical intuition.

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

For $m_2 \gg m_1$:

$$
\boxed{v_1 \approx -u_1+2u_2,\qquad v_2 \approx u_2}
$$
