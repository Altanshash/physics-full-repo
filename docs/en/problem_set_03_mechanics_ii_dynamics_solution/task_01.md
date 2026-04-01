## Problem 1 – Newton’s second law (constant force)

### Given

A constant force acts on a body of mass

$$
m = 2 \text{ kg}
$$

$$
\vec{F} = (6, 2) \text{ N}
$$

Initial conditions:

$$
\vec{v}(0) = (1, -1), \qquad \vec{r}(0) = (0, 0)
$$

---

## 1. Acceleration $\vec{a}(t)$

Using Newton’s second law:

$$
\vec{F} = m \vec{a}
$$

So,

$$
\vec{a} = \frac{\vec{F}}{m}
= \left(\frac{6}{2}, \frac{2}{2}\right)
= (3, 1)
$$

Thus,

$$
\vec{a}(t) = (3, 1)
$$

---

## 2. Velocity $\vec{v}(t)$

Velocity is obtained by integrating acceleration:

$$
\vec{v}(t) = \vec{v}(0) + \int_0^t \vec{a}\,d\tau
$$

Since acceleration is constant:

$$
\vec{v}(t) = (1, -1) + (3t, t)
$$

So,

$$
\vec{v}(t) = (1 + 3t, -1 + t)
$$

---

## 3. Position $\vec{r}(t)$

Position is obtained by integrating velocity:

$$
\vec{r}(t) = \vec{r}(0) + \int_0^t \vec{v}(\tau)\,d\tau
$$

Since $\vec{r}(0) = (0,0)$, we get

$$
\vec{r}(t) = \int_0^t (1 + 3\tau,\,-1 + \tau)\,d\tau
$$

Integrate each component:

$$
\int_0^t (1 + 3\tau)\,d\tau = t + \frac{3}{2}t^2
$$

$$
\int_0^t (-1 + \tau)\,d\tau = -t + \frac{1}{2}t^2
$$

Thus,

$$
\vec{r}(t) = \left(t + \frac{3}{2}t^2,\,-t + \frac{1}{2}t^2\right)
$$

---

## 4. Trajectory

From

$$
x(t) = t + \frac{3}{2}t^2, \qquad
y(t) = -t + \frac{1}{2}t^2
$$

the motion follows a **parabolic trajectory** in the plane.

---

## 5. Work done at $t = 3$

Work is

$$
W = \vec{F} \cdot \vec{s}
$$

where displacement

$$
\vec{s} = \vec{r}(3) - \vec{r}(0) = \vec{r}(3)
$$

Compute position at $t=3$:

$$
x(3) = 3 + \frac{3}{2}\cdot 9 = 3 + 13.5 = 16.5
$$

$$
y(3) = -3 + \frac{1}{2}\cdot 9 = -3 + 4.5 = 1.5
$$

So,

$$
\vec{s} = (16.5, 1.5)
$$

Now compute work:

$$
W = (6, 2) \cdot (16.5, 1.5)
= 6 \cdot 16.5 + 2 \cdot 1.5
$$

$$
W = 99 + 3 = 102
$$

Thus,

$$
W = 102 \text{ J}
$$

---

## 6. Work-energy theorem check

Kinetic energy:

$$
K = \frac{1}{2} m v^2
$$

Initial velocity:

$$
|\vec{v}(0)|^2 = 1^2 + (-1)^2 = 2
$$

$$
K_0 = \frac{1}{2} \cdot 2 \cdot 2 = 2
$$

Velocity at $t=3$:

$$
\vec{v}(3) = (1+9, -1+3) = (10, 2)
$$

$$
|\vec{v}(3)|^2 = 10^2 + 2^2 = 104
$$

$$
K = \frac{1}{2} \cdot 2 \cdot 104 = 104
$$

Change in kinetic energy:

$$
\Delta K = 104 - 2 = 102
$$

Thus,

$$
W = \Delta K = 102
$$

✔ The work-energy theorem is satisfied.

---

## Final answers

$$
\vec{a}(t) = (3, 1)
$$

$$
\vec{v}(t) = (1 + 3t, -1 + t)
$$

$$
\vec{r}(t) = \left(t + \frac{3}{2}t^2,\,-t + \frac{1}{2}t^2\right)
$$

$$
W = 102 \text{ J}
$$
