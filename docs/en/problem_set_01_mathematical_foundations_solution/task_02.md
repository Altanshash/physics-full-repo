## Problem 2 – Parametric trajectory, velocity, and acceleration

### Given

The trajectory is given by

$$
\vec{r}(t) = (t^2,\sin t,5).
$$

We need to determine:

- the velocity vector $\vec{v}(t)$,
- the acceleration vector $\vec{a}(t)$,
- the value of $|\vec{v}(1)|$,
- the dot product $\vec{v}\cdot\vec{a}$,
- the cross product $\vec{v}\times\vec{a}$.

---

## 1. Velocity vector

The velocity is the derivative of the position vector:

$$
\vec{v}(t)=\frac{d\vec{r}}{dt}.
$$

Since

$$
\vec{r}(t)=(t^2,\sin t,5),
$$

we differentiate each component:

$$
\frac{d}{dt}(t^2)=2t,
\qquad
\frac{d}{dt}(\sin t)=\cos t,
\qquad
\frac{d}{dt}(5)=0.
$$

Therefore,

$$
\boxed{\vec{v}(t)=(2t,\cos t,0)}.
$$

---

## 2. Acceleration vector

The acceleration is the derivative of the velocity vector:

$$
\vec{a}(t)=\frac{d\vec{v}}{dt}.
$$

Using

$$
\vec{v}(t)=(2t,\cos t,0),
$$

we differentiate again:

$$
\frac{d}{dt}(2t)=2,
\qquad
\frac{d}{dt}(\cos t)=-\sin t,
\qquad
\frac{d}{dt}(0)=0.
$$

So we obtain

$$
\boxed{\vec{a}(t)=(2,-\sin t,0)}.
$$

---

## 3. Magnitude of the velocity at $t=1$

First compute the velocity at $t=1$:

$$
\vec{v}(1)=(2\cdot 1,\cos 1,0)=(2,\cos 1,0).
$$

The magnitude of a vector $(x,y,z)$ is

$$
|(x,y,z)|=\sqrt{x^2+y^2+z^2}.
$$

Hence,

$$
|\vec{v}(1)|
=
\sqrt{2^2+(\cos 1)^2+0^2}
=
\sqrt{4+\cos^2 1}.
$$

Therefore,

$$
\boxed{|\vec{v}(1)|=\sqrt{4+\cos^2 1}}.
$$

Using $\cos 1\approx 0.5403$, we get

$$
|\vec{v}(1)|\approx \sqrt{4.2919}\approx 2.07.
$$

So,

$$
\boxed{|\vec{v}(1)|\approx 2.07}.
$$

---

## 4. Dot product $\vec{v}\cdot\vec{a}$

We have

$$
\vec{v}(t)=(2t,\cos t,0),
\qquad
\vec{a}(t)=(2,-\sin t,0).
$$

The dot product is found by multiplying corresponding components and adding them:

$$
\vec{v}\cdot\vec{a}
=
(2t)(2)+(\cos t)(-\sin t)+0\cdot 0.
$$

Simplifying gives

$$
\vec{v}\cdot\vec{a}=4t-\sin t\cos t.
$$

Thus,

$$
\boxed{\vec{v}\cdot\vec{a}=4t-\sin t\cos t}.
$$

---

## 5. Cross product $\vec{v}\times\vec{a}$

For two vectors

$$
(u_1,u_2,u_3)\times(w_1,w_2,w_3)
=
\left(
u_2w_3-u_3w_2,\;
u_3w_1-u_1w_3,\;
u_1w_2-u_2w_1
\right).
$$

Here,

$$
\vec{v}(t)=(2t,\cos t,0),
\qquad
\vec{a}(t)=(2,-\sin t,0).
$$

Now compute each component.

### First component

$$
v_2a_3-v_3a_2
=
(\cos t)(0)-(0)(-\sin t)=0.
$$

### Second component

$$
v_3a_1-v_1a_3
=
(0)(2)-(2t)(0)=0.
$$

### Third component

$$
v_1a_2-v_2a_1
=
(2t)(-\sin t)-(\cos t)(2).
$$

So,

$$
v_1a_2-v_2a_1=-2t\sin t-2\cos t.
$$

Therefore,

$$
\boxed{\vec{v}\times\vec{a}=(0,0,-2t\sin t-2\cos t)}.
$$

We may also write it as

$$
\boxed{\vec{v}\times\vec{a}=(0,0,-2(t\sin t+\cos t))}.
$$

---

## Final answers

$$
\boxed{\vec{v}(t)=(2t,\cos t,0)}
$$

$$
\boxed{\vec{a}(t)=(2,-\sin t,0)}
$$

$$
\boxed{|\vec{v}(1)|=\sqrt{4+\cos^2 1}\approx 2.07}
$$

$$
\boxed{\vec{v}\cdot\vec{a}=4t-\sin t\cos t}
$$

$$
\boxed{\vec{v}\times\vec{a}=(0,0,-2t\sin t-2\cos t)}
$$
