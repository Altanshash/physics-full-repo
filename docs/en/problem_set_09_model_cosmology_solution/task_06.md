# Problem 6 – Two-body Motion and the Barycenter

## Given

We consider two bodies with masses $m_1$ and $m_2$.

Their position vectors are $r_1$ and $r_2$.

The barycenter is:

$$R=\frac{m_1r_1+m_2r_2}{m_1+m_2}$$

For an isolated system:

$$m_1r_1+m_2r_2=\text{constant}$$

The equations of motion are:

$$m_1\ddot{r}_1=-\frac{Gm_1m_2(r_1-r_2)}{|r_1-r_2|^3}$$

$$m_2\ddot{r}_2=-\frac{Gm_1m_2(r_2-r_1)}{|r_2-r_1|^3}$$

---

## Solution

### 1. Center of Mass

The center of mass is:

$$R=\frac{m_1r_1+m_2r_2}{m_1+m_2}$$

If $m_1=m_2$, the barycenter is exactly between the two bodies.

If $m_1>m_2$, the barycenter is closer to body 1.

If $m_1<m_2$, the barycenter is closer to body 2.

---

### 2. Isolated System

For an isolated system, there is no external force.

Therefore, the center of mass remains constant.

$$m_1r_1+m_2r_2=\text{constant}$$

If the barycenter is chosen as the origin:

$$R=0$$

Then:

$$m_1r_1+m_2r_2=0$$

---

### 3. Equations of Motion

For body 1:

$$m_1\ddot{r}_1=-\frac{Gm_1m_2(r_1-r_2)}{|r_1-r_2|^3}$$

For body 2:

$$m_2\ddot{r}_2=-\frac{Gm_1m_2(r_2-r_1)}{|r_2-r_1|^3}$$

The forces are equal and opposite:

$$F_1+F_2=0$$

So the barycenter remains fixed.

---

### 4. Dependence on Mass Ratio

The distances from the barycenter satisfy:

$$m_1r_1=m_2r_2$$

Therefore:

$$\frac{r_1}{r_2}=\frac{m_2}{m_1}$$

If $m_1\gg m_2$, the heavier body moves only slightly.

If $m_1=m_2$, both bodies move in equal-size orbits.

---

## HTML Requirements

The HTML visualization should include:

- trajectories of both bodies
- marked barycenter
- mass ratio slider

---

## Conclusion

In a two-body gravitational system, both bodies orbit around their common barycenter.

The barycenter is:

$$R=\frac{m_1r_1+m_2r_2}{m_1+m_2}$$

For an isolated system:

$$m_1r_1+m_2r_2=\text{constant}$$

The orbit sizes depend on the mass ratio:

$$\frac{r_1}{r_2}=\frac{m_2}{m_1}$$

Thus, the heavier body moves in a smaller orbit, while the lighter body moves in a larger orbit.
