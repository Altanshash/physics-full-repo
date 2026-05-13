# Problem 6 – Two-body Motion and the Barycenter

## Given

We consider two bodies with masses $m_1$ and $m_2$.

Their position vectors are:

- $\vec{r}_1$ for body 1
- $\vec{r}_2$ for body 2

The center of mass, or barycenter, is defined as:

$$
\vec{R}=\frac{m_1\vec{r}_1+m_2\vec{r}_2}{m_1+m_2}
$$

For an isolated system:

$$
m_1\vec{r}_1+m_2\vec{r}_2=\text{constant}
$$

The equations of motion are:

$$
m_1\ddot{\vec{r}}_1
=
-G\frac{m_1m_2}{|\vec{r}_1-\vec{r}_2|^3}
(\vec{r}_1-\vec{r}_2)
$$

$$
m_2\ddot{\vec{r}}_2
=
-G\frac{m_1m_2}{|\vec{r}_2-\vec{r}_1|^3}
(\vec{r}_2-\vec{r}_1)
$$

---

## Solution

### 1. Center of Mass

The barycenter of two bodies is:

$$
\vec{R}=\frac{m_1\vec{r}_1+m_2\vec{r}_2}{m_1+m_2}
$$

This point represents the average position of the system weighted by mass.

If $m_1=m_2$, the barycenter is exactly between the two bodies.

If $m_1>m_2$, the barycenter is closer to body 1.

If $m_1<m_2$, the barycenter is closer to body 2.

---

### 2. Isolated System

For an isolated two-body system, no external force acts on the system.

Therefore, the center of mass remains constant or moves with constant velocity.

If the barycenter is chosen as the origin, then:

$$
\vec{R}=0
$$

So:

$$
m_1\vec{r}_1+m_2\vec{r}_2=0
$$

This shows that the two bodies move around their common barycenter.

---

### 3. Equations of Motion

The gravitational force between the two bodies is given by Newton's law of gravitation.

For body 1:

$$
m_1\ddot{\vec{r}}_1
=
-G\frac{m_1m_2}{|\vec{r}_1-\vec{r}_2|^3}
(\vec{r}_1-\vec{r}_2)
$$

For body 2:

$$
m_2\ddot{\vec{r}}_2
=
-G\frac{m_1m_2}{|\vec{r}_2-\vec{r}_1|^3}
(\vec{r}_2-\vec{r}_1)
$$

The forces are equal in magnitude and opposite in direction.

Therefore, the total internal force is zero:

$$
\vec{F}_1+\vec{F}_2=0
$$

This keeps the barycenter fixed for an isolated system.

---

### 4. Dependence on Mass Ratio

The position of each body relative to the barycenter depends on the mass ratio.

The distances from the barycenter satisfy:

$$
m_1r_1=m_2r_2
$$

Therefore:

$$
\frac{r_1}{r_2}=\frac{m_2}{m_1}
$$

If $m_1$ is much larger than $m_2$, body 1 moves in a small orbit while body 2 moves in a large orbit.

If the masses are equal, both bodies move in orbits of equal size around the barycenter.

---

## HTML Requirements

The HTML visualization should include:

- Trajectories of both bodies
- Marked barycenter
- Mass ratio slider

---

## Conclusion

In a two-body gravitational system, both bodies orbit around their common center of mass, called the barycenter.

The barycenter is given by:

$$
\vec{R}=\frac{m_1\vec{r}_1+m_2\vec{r}_2}{m_1+m_2}
$$

For an isolated system, the barycenter remains fixed or moves uniformly.

The sizes of the two orbits depend on the mass ratio:

$$
\frac{r_1}{r_2}=\frac{m_2}{m_1}
$$

Thus, when one mass is much larger, the larger body moves only slightly, while the smaller body makes a much larger orbit.
