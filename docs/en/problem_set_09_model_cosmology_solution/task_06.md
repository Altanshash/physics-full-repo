# Problem 6 – Two-body Motion and the Barycenter

## Given

We consider two bodies with masses $m_1$ and $m_2$.

Their position vectors are:

- $\vec{r}_1$ for body 1
- $\vec{r}_2$ for body 2

The barycenter, or center of mass, is:

$$
R = \frac{m_1 r_1 + m_2 r_2}{m_1 + m_2}
$$

For an isolated system:

$$
m_1 r_1 + m_2 r_2 = \text{constant}
$$

The equations of motion are:

$$
m_1 \ddot{r}_1
=
-\frac{G m_1 m_2 (r_1-r_2)}
{|r_1-r_2|^3}
$$

$$
m_2 \ddot{r}_2
=
-\frac{G m_1 m_2 (r_2-r_1)}
{|r_2-r_1|^3}
$$

---

# Solution

## 1. Center of Mass

The barycenter is defined as:

$$
R = \frac{m_1 r_1 + m_2 r_2}{m_1 + m_2}
$$

This point is the mass-weighted average position of the system.

If:

$$
m_1 = m_2
$$

the barycenter lies exactly between the two bodies.

If:

$$
m_1 > m_2
$$

the barycenter is closer to body 1.

If:

$$
m_1 < m_2
$$

the barycenter is closer to body 2.

---

## 2. Isolated System

For an isolated system, there is no external force.

Therefore, the barycenter remains fixed or moves with constant velocity.

If the barycenter is chosen as the origin:

$$
R = 0
$$

then:

$$
m_1 r_1 + m_2 r_2 = 0
$$

This means both bodies move around their common barycenter.

---

## 3. Equations of Motion

The gravitational force acting on body 1 is:

$$
m_1 \ddot{r}_1
=
-\frac{G m_1 m_2 (r_1-r_2)}
{|r_1-r_2|^3}
$$

The gravitational force acting on body 2 is:

$$
m_2 \ddot{r}_2
=
-\frac{G m_1 m_2 (r_2-r_1)}
{|r_2-r_1|^3}
$$

The forces are equal in magnitude and opposite in direction.

Therefore:

$$
F_1 + F_2 = 0
$$

which keeps the barycenter fixed.

---

## 4. Dependence on Mass Ratio

The distances from the barycenter satisfy:

$$
m_1 r_1 = m_2 r_2
$$

Therefore:

$$
\frac{r_1}{r_2}
=
\frac{m_2}{m_1}
$$

If:

$$
m_1 \gg m_2
$$

body 1 moves in a very small orbit, while body 2 moves in a much larger orbit.

If:

$$
m_1 = m_2
$$

both bodies move in equal-size orbits.

---

# HTML Requirements

The HTML visualization should include:

- trajectories of both bodies
- marked barycenter
- mass ratio slider

---

# Conclusion

In a two-body gravitational system, both bodies orbit around their common center of mass.

The barycenter is:

$$
R = \frac{m_1 r_1 + m_2 r_2}{m_1 + m_2}
$$

For an isolated system:

$$
m_1 r_1 + m_2 r_2 = \text{constant}
$$

The orbit sizes depend on the mass ratio:

$$
\frac{r_1}{r_2}
=
\frac{m_2}{m_1}
$$

Thus, if one body is much heavier, it moves only slightly, while the lighter body moves in a much larger orbit around the barycenter.
