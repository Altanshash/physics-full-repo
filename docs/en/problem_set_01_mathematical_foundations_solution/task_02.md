## Problem 2 – Parametric trajectory

### Given

The trajectory is

$$
\vec{r}(t) = (t^2, \sin t, 5)
$$

---

## 1. Velocity

Velocity is the derivative of position:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt}
$$

Differentiate each component:

$$
\vec{v}(t) = (2t, \cos t, 0)
$$

---

## 2. Acceleration

Acceleration is the derivative of velocity:

$$
\vec{a}(t) = \frac{d\vec{v}}{dt}
$$

$$
\vec{a}(t) = (2, -\sin t, 0)
$$

---

## 3. Speed at $t=1$

$$
\vec{v}(1) = (2, \cos 1, 0)
$$

$$
|\vec{v}(1)| = \sqrt{2^2 + \cos^2 1}
= \sqrt{4 + \cos^2 1}
$$

$$
|\vec{v}(1)| \approx 2.07
$$

---

## 4. Dot product

$$
\vec{v}\cdot\vec{a}
= (2t)(2) + (\cos t)(-\sin t)
$$

$$
\vec{v}\cdot\vec{a} = 4t - \sin t \cos t
$$

---

## 5. Cross product

Use component formula:

$$
\vec{v} = (2t, \cos t, 0), \quad
\vec{a} = (2, -\sin t, 0)
$$

First component:

$$
(\cos t)(0) - (0)(-\sin t) = 0
$$

Second component:

$$
(0)(2) - (2t)(0) = 0
$$

Third component:

$$
(2t)(-\sin t) - (\cos t)(2)
= -2t\sin t - 2\cos t
$$

Final result:

$$
\vec{v}\times\vec{a} = (0, 0, -2t\sin t - 2\cos t)
$$

---

## Final answers

$$
\vec{v}(t) = (2t, \cos t, 0)
$$

$$
\vec{a}(t) = (2, -\sin t, 0)
$$

$$
|\vec{v}(1)| \approx 2.07
$$

$$
\vec{v}\cdot\vec{a} = 4t - \sin t \cos t
$$

$$
\vec{v}\times\vec{a} = (0, 0, -2t\sin t - 2\cos t)
$$
