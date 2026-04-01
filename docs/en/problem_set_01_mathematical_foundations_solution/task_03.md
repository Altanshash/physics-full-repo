## Problem 3 – Integration of motion

### Given

We solve the problem in two parts.

---

## A) For a given velocity

We are given

$$
\vec{v}(t) = (2t,\ 3,\ -e^{-t}),
\qquad
\vec{r}(0) = (0,\ 1,\ 2).
$$

We need to determine:

1. the position vector $\vec{r}(t)$,
2. the acceleration vector $\vec{a}(t)$.

---

### 1. Position vector $\vec{r}(t)$

The position is found from

$$
\vec{r}(t)=\vec{r}(0)+\int_0^t \vec{v}(\tau)\,d\tau.
$$

Substitute the given data:

$$
\vec{r}(t)
=
(0,1,2)
+
\int_0^t (2\tau,\ 3,\ -e^{-\tau})\,d\tau.
$$

Now integrate each component separately.

For the first component:

$$
\int_0^t 2\tau\,d\tau
=
\left[\tau^2\right]_0^t
=
t^2.
$$

For the second component:

$$
\int_0^t 3\,d\tau
=
\left[3\tau\right]_0^t
=
3t.
$$

For the third component:

$$
\int_0^t -e^{-\tau}\,d\tau
=
\left[e^{-\tau}\right]_0^t
=
e^{-t}-1.
$$

So,

$$
\vec{r}(t)
=
(0,1,2)
+
(t^2,\ 3t,\ e^{-t}-1).
$$

Add the vectors componentwise:

$$
\vec{r}(t)
=
\left(
t^2,\ 1+3t,\ 2+e^{-t}-1
\right).
$$

Hence,

$$
\boxed{
\vec{r}(t)=\left(t^2,\ 1+3t,\ 1+e^{-t}\right)
}.
$$

#### Check at $t=0$

$$
\vec{r}(0)=\left(0,\ 1,\ 1+e^0\right)=(0,1,2),
$$

which agrees with the given initial condition.

---

### 2. Acceleration vector $\vec{a}(t)$

Acceleration is the derivative of velocity:

$$
\vec{a}(t)=\frac{d\vec{v}}{dt}.
$$

Since

$$
\vec{v}(t)=(2t,\ 3,\ -e^{-t}),
$$

differentiate each component:

$$
\frac{d}{dt}(2t)=2,
\qquad
\frac{d}{dt}(3)=0,
\qquad
\frac{d}{dt}(-e^{-t})=e^{-t}.
$$

Therefore,

$$
\boxed{
\vec{a}(t)=(2,\ 0,\ e^{-t})
}.
$$

---

## B) For a given acceleration

We are given

$$
\vec{a}(t)=(4,\ -\sin t,\ 0),
\qquad
\vec{v}(0)=(1,\ 0,\ 2),
\qquad
\vec{r}(0)=(0,\ 0,\ 0).
$$

We need to determine:

1. the velocity vector $\vec{v}(t)$,
2. the position vector $\vec{r}(t)$.

---

### 1. Velocity vector $\vec{v}(t)$

The velocity is found from

$$
\vec{v}(t)=\vec{v}(0)+\int_0^t \vec{a}(\tau)\,d\tau.
$$

Substitute the given acceleration:

$$
\vec{v}(t)
=
(1,0,2)
+
\int_0^t (4,\ -\sin\tau,\ 0)\,d\tau.
$$

Now integrate componentwise.

For the first component:

$$
\int_0^t 4\,d\tau
=
4t.
$$

For the second component:

$$
\int_0^t -\sin\tau\,d\tau
=
\left[\cos\tau\right]_0^t
=
\cos t-1.
$$

For the third component:

$$
\int_0^t 0\,d\tau
=
0.
$$

Thus,

$$
\vec{v}(t)
=
(1,0,2)
+
(4t,\ \cos t-1,\ 0).
$$

Add the vectors:

$$
\vec{v}(t)
=
\left(
1+4t,\ \cos t-1,\ 2
\right).
$$

So,

$$
\boxed{
\vec{v}(t)=\left(1+4t,\ \cos t-1,\ 2\right)
}.
$$

#### Check at $t=0$

$$
\vec{v}(0)=\left(1,\ \cos 0-1,\ 2\right)=(1,0,2),
$$

which matches the given initial condition.

---

### 2. Position vector $\vec{r}(t)$

Now use

$$
\vec{r}(t)=\vec{r}(0)+\int_0^t \vec{v}(\tau)\,d\tau.
$$

Since

$$
\vec{r}(0)=(0,0,0),
$$

we get

$$
\vec{r}(t)
=
\int_0^t (1+4\tau,\ \cos\tau-1,\ 2)\,d\tau.
$$

Integrate each component.

For the first component:

$$
\int_0^t (1+4\tau)\,d\tau
=
\left[\tau+2\tau^2\right]_0^t
=
t+2t^2.
$$

For the second component:

$$
\int_0^t (\cos\tau-1)\,d\tau
=
\left[\sin\tau-\tau\right]_0^t
=
\sin t-t.
$$

For the third component:

$$
\int_0^t 2\,d\tau
=
2t.
$$

Therefore,

$$
\boxed{
\vec{r}(t)=\left(t+2t^2,\ \sin t-t,\ 2t\right)
}.
$$

#### Check at $t=0$

$$
\vec{r}(0)=\left(0,\ 0,\ 0\right),
$$

so the initial condition is satisfied.

---

## Final answers

### Part A

$$
\boxed{
\vec{r}(t)=\left(t^2,\ 1+3t,\ 1+e^{-t}\right)
}
$$

$$
\boxed{
\vec{a}(t)=(2,\ 0,\ e^{-t})
}
$$

### Part B

$$
\boxed{
\vec{v}(t)=\left(1+4t,\ \cos t-1,\ 2\right)
}
$$

$$
\boxed{
\vec{r}(t)=\left(t+2t^2,\ \sin t-t,\ 2t\right)
}
$$
