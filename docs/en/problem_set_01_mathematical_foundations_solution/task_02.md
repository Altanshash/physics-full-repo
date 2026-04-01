## Problem 2 – Parametric trajectory, velocity, and acceleration

### Given

The trajectory is given by

$$
\vec{r}(t) = (t^2, \sin t, 5)
$$

---

## 1. Velocity vector

The velocity is the derivative of the position:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt}
$$

Differentiate each component:

$$
\vec{v}(t) = (2t, \cos t, 0)
$$

---

## 2. Acceleration vector

The acceleration is the derivative of velocity:

$$
\vec{a}(t) = \frac{d\vec{v}}{dt}
$$

Differentiate again:

$$
\vec{a}(t) = (2, -\sin t, 0)
$$

---

## 3. Speed at $t=1$

First compute velocity:

$$
\vec{v}(1) = (2, \cos 1, 0)
$$

Magnitude:

$$
|\vec{v}(1)| = \sqrt{2^2 + (\cos 1)^2}
= \sqrt{4 + \cos^2 1}
$$

Approximation:

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

We compute

$$
\vec{v}\times\vec{a}
=
\begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
2t & \cos t & 0 \\
2 & -\sin t & 0
\end{vmatrix}
$$

Expand:

$$
\vec{v}\times\vec{a}
=
\mathbf{i}
\begin{vmatrix}
\cos t & 0 \\
-\sin t & 0
\end{vmatrix}
-
\mathbf{j}
\begin{vmatrix}
2t & 0 \\
2 & 0
\end{vmatrix}
+
\mathbf{k}
\begin{vmatrix}
2t & \cos t \\
2 & -\sin t
\end{vmatrix}
$$

First two determinants:

$$
\begin{vmatrix}
\cos t & 0 \\
-\sin t & 0
\end{vmatrix}
= 0
$$

$$
\begin{vmatrix}
2t & 0 \\
2 & 0
\end{vmatrix}
= 0
$$

Last determinant:

$$
\begin{vmatrix}
2t & \cos t \\
2 & -\sin t
\end{vmatrix}
= (2t)(-\sin t) - (\cos t)(2)
$$

$$
= -2t\sin t - 2\cos t
$$

Therefore,

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
|\vec{v}(1)| = \sqrt{4 + \cos^2 1} \approx 2.07
$$

$$
\vec{v}\cdot\vec{a} = 4t - \sin t \cos t
$$

$$
\vec{v}\times\vec{a} = (0, 0, -2t\sin t - 2\cos t)
$$
