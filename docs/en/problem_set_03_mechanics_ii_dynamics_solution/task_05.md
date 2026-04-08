## Problem 5 – Momentum and one-dimensional head-on collision

### Given

Two bodies with masses $m_1$ and $m_2$ move along one straight line.  
The collision is elastic.

Initial velocities:

$$
u_1,\qquad u_2
$$

Final velocities:

$$
v_1,\qquad v_2
$$

---

## 1. Conservation laws

For an elastic one-dimensional collision, momentum and kinetic energy are conserved:

$$
m_1u_1 + m_2u_2 = m_1v_1 + m_2v_2
$$

$$
\frac{1}{2}m_1u_1^2 + \frac{1}{2}m_2u_2^2
=
\frac{1}{2}m_1v_1^2 + \frac{1}{2}m_2v_2^2
$$

A useful additional relation is

$$
u_1 - u_2 = -(v_1 - v_2)
$$

or

$$
u_1 - u_2 = v_2 - v_1
$$

---

## 2. Velocities after the collision

From the relative velocity relation,

$$
v_2 = v_1 + u_1 - u_2
$$

Substitute this into momentum conservation:

$$
m_1u_1 + m_2u_2 = m_1v_1 + m_2(v_1 + u_1 - u_2)
$$

Expand:

$$
m_1u_1 + m_2u_2 = (m_1+m_2)v_1 + m_2u_1 - m_2u_2
$$

Rearrange:

$$
(m_1-m_2)u_1 + 2m_2u_2 = (m_1+m_2)v_1
$$

Hence,

$$
\boxed{
v_1 = \frac{(m_1-m_2)u_1 + 2m_2u_2}{m_1+m_2}
}
$$

Now use

$$
v_2 = v_1 + u_1 - u_2
$$

After simplification,

$$
\boxed{
v_2 = \frac{2m_1u_1 + (m_2-m_1)u_2}{m_1+m_2}
}
$$

---

## 3. Case $m_1 = m_2$

Let

$$
m_1 = m_2 = m
$$

Then

$$
v_1 = \frac{(m-m)u_1 + 2mu_2}{2m} = u_2
$$

$$
v_2 = \frac{2mu_1 + (m-m)u_2}{2m} = u_1
$$

So, for equal masses, the bodies exchange velocities:

$$
\boxed{v_1 = u_2,\qquad v_2 = u_1}
$$

---

## 4. Limit case $m_2 \gg m_1$

From the formula for $v_1$:

$$
v_1 = \frac{(m_1-m_2)u_1 + 2m_2u_2}{m_1+m_2}
$$

if $m_2 \gg m_1$, then approximately

$$
\boxed{v_1 \approx -u_1 + 2u_2}
$$

From the formula for $v_2$:

$$
v_2 = \frac{2m_1u_1 + (m_2-m_1)u_2}{m_1+m_2}
$$

if $m_2 \gg m_1$, then

$$
\boxed{v_2 \approx u_2}
$$

A common special case is $u_2=0$. Then

$$
\boxed{v_1 \approx -u_1,\qquad v_2 \approx 0}
$$

---

## 5. Physical interpretation

- In an elastic collision, both momentum and kinetic energy are conserved.
- If the masses are equal, the bodies swap velocities.
- If one body is much heavier, its velocity changes very little.
- A light body hitting a very heavy body behaves almost like a ball bouncing from a wall.

---

## Final answers

$$
\boxed{
v_1 = \frac{(m_1-m_2)u_1 + 2m_2u_2}{m_1+m_2}
}
$$

$$
\boxed{
v_2 = \frac{2m_1u_1 + (m_2-m_1)u_2}{m_1+m_2}
}
$$

$$
\boxed{v_1 = u_2,\qquad v_2 = u_1 \text{ when } m_1=m_2}
$$

$$
\boxed{v_1 \approx -u_1 + 2u_2,\qquad v_2 \approx u_2 \text{ when } m_2 \gg m_1}
$$
