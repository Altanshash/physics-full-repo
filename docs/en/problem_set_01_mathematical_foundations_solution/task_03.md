## Problem 3 – Integration of motion

### A) For a given velocity

Given:

$$
\vec{v}(t) = (2t, 3, -e^{-t}), \qquad \vec{r}(0) = (0, 1, 2)
$$

We need to determine:

1. the position vector $\vec{r}(t)$,
2. the acceleration vector $\vec{a}(t)$.

---

### 1. Position vector

We use the formula

$$
\vec{r}(t) = \vec{r}(0) + \int_0^t \vec{v}(\tau)\,d\tau.
$$

Substitute the given velocity:

$$
\vec{r}(t) = (0,1,2) + \int_0^t (2\tau, 3, -e^{-\tau})\,d\tau.
$$

Now integrate each component separately:

$$
\int_0^t 2\tau\,d\tau = t^2
$$

$$
\int_0^t 3\,d\tau = 3t
$$

$$
\int_0^t -e^{-\tau}\,d\tau = e^{-t} - 1
$$

Therefore,

$$
\vec{r}(t) = (0,1,2) + (t^2, 3t, e^{-t} - 1)
$$

So,

$$
\vec{r}(t) = (t^2, 1 + 3t, 1 + e^{-t})
$$

---

### 2. Acceleration vector

Acceleration is the derivative of velocity:

$$
\vec{a}(t) = \frac{d\vec{v}}{dt}
$$

Differentiate each component of

$$
\vec{v}(t) = (2t, 3, -e^{-t})
$$

We get:

$$
\vec{a}(t) = (2, 0, e^{-t})
$$

---

## B) For a given acceleration

Given:

$$
\vec{a}(t) = (4, -\sin t, 0), \qquad \vec{v}(0) = (1,0,2), \qquad \vec{r}(0) = (0,0,0)
$$

We need to determine:

1. the velocity vector $\vec{v}(t)$,
2. the position vector $\vec{r}(t)$.

---

### 1. Velocity vector

We use

$$
\vec{v}(t) = \vec{v}(0) + \int_0^t \vec{a}(\tau)\,d\tau
$$

Substitute the given acceleration:

$$
\vec{v}(t) = (1,0,2) + \int_0^t (4, -\sin \tau, 0)\,d\tau
$$

Integrate each component:

$$
\int_0^t 4\,d\tau = 4t
$$

$$
\int_0^t -\sin \tau\,d\tau = \cos t - 1
$$

$$
\int_0^t 0\,d\tau = 0
$$

Therefore,

$$
\vec{v}(t) = (1,0,2) + (4t, \cos t - 1, 0)
$$

So,

$$
\vec{v}(t) = (1 + 4t, \cos t - 1, 2)
$$

---

### 2. Position vector

Now use

$$
\vec{r}(t) = \vec{r}(0) + \int_0^t \vec{v}(\tau)\,d\tau
$$

Since $\vec{r}(0) = (0,0,0)$, we get

$$
\vec{r}(t) = \int_0^t (1 + 4\tau, \cos \tau - 1, 2)\,d\tau
$$

Integrate each component:

$$
\int_0^t (1 + 4\tau)\,d\tau = t + 2t^2
$$

$$
\int_0^t (\cos \tau - 1)\,d\tau = \sin t - t
$$

$$
\int_0^t 2\,d\tau = 2t
$$

Therefore,

$$
\vec{r}(t) = (t + 2t^2, \sin t - t, 2t)
$$

---

## Final answers

### Part A

$$
\vec{r}(t) = (t^2, 1 + 3t, 1 + e^{-t})
$$

$$
\vec{a}(t) = (2, 0, e^{-t})
$$

### Part B

$$
\vec{v}(t) = (1 + 4t, \cos t - 1, 2)
$$

$$
\vec{r}(t) = (t + 2t^2, \sin t - t, 2t)
$$
