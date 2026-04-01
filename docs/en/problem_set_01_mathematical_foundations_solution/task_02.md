## Problem 2 – Parametric trajectory, velocity, and acceleration

### Given

The trajectory is given in parametric form by

$$
\vec{r}(t)=(t^2,\sin t,5).
$$

We need to:

1. determine the velocity vector $$\vec{v}(t)=\dfrac{d\vec{r}}{dt}$$,
2. determine the acceleration vector $$\vec{a}(t)=\dfrac{d^2\vec{r}}{dt^2}$$,
3. calculate $$|\vec{v}(1)|$$,
4. calculate $$\vec{v}\cdot\vec{a}$$,
5. calculate $$\vec{v}\times\vec{a}$$.

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

we differentiate each component separately:

- $$\dfrac{d}{dt}(t^2)=2t,$$
- $$\dfrac{d}{dt}(\sin t)=\cos t,$$
- $$\dfrac{d}{dt}(5)=0.$$

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

we again differentiate component by component:

- $$\dfrac{d}{dt}(2t)=2,$$
- $$\dfrac{d}{dt}(\cos t)=-\sin t,$$
- $$\dfrac{d}{dt}(0)=0.$$

So,

$$
\boxed{\vec{a}(t)=(2,-\sin t,0)}.
$$

---

## 3. Speed at $$t=1$$

First evaluate the velocity vector at $$t=1$$:

$$
\vec{v}(1)=(2\cdot1,\cos1,0)=(2,\cos1,0).
$$

The magnitude of a vector $$(x,y,z)$$ is

$$
|(x,y,z)|=\sqrt{x^2+y^2+z^2}.
$$

Hence,

$$
|\vec{v}(1)|=\sqrt{2^2+(\cos1)^2+0^2}.
$$

So we get

$$
|\vec{v}(1)|=\sqrt{4+\cos^2 1}.
$$

Therefore,

$$
\boxed{|\vec{v}(1)|=\sqrt{4+\cos^2 1}}.
$$

Numerically,

$$
\cos 1 \approx 0.5403,
\qquad
\cos^2 1 \approx 0.2919,
$$

thus

$$
|\vec{v}(1)|\approx \sqrt{4.2919}\approx 2.07.
$$

So,

$$
\boxed{|\vec{v}(1)|\approx 2.07}.
$$

---

## 4. Dot product $$\vec{v}\cdot\vec{a}$$

We use the formulas

$$
\vec{v}(t)=(2t,\cos t,0),
\qquad
\vec{a}(t)=(2,-\sin t,0).
$$

The dot product is

$$
\vec{v}\cdot\vec{a}
=(2t)(2)+(\cos t)(-\sin t)+0\cdot0.
$$

This simplifies to

$$
\vec{v}\cdot\vec{a}=4t-\sin t\cos t.
$$

Hence,

$$
\boxed{\vec{v}\cdot\vec{a}=4t-\sin t\cos t}.
$$

---

## 5. Cross product $$\vec{v}\times\vec{a}$$

We compute

$$
\vec{v}\times\vec{a}
=
\begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
2t & \cos t & 0 \\
2 & -\sin t & 0
\end{vmatrix}.
$$

Now expand the determinant:

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
\end{vmatrix}.
$$

The first two determinants are zero:

$$
\begin{vmatrix}
\cos t & 0 \\
-\sin t & 0
\end{vmatrix}=0,
\qquad
\begin{vmatrix}
2t & 0 \\
2 & 0
\end{vmatrix}=0.
$$

For the last one:

$$
\begin{vmatrix}
2t & \cos t \\
2 & -\sin t
\end{vmatrix}
=(2t)(-\sin t)-(\cos t)(2)
=-2t\sin t-2\cos t.
$$

Therefore,

$$
\vec{v}\times\vec{a}=(0,0,-2t\sin t-2\cos t).
$$

So,

$$
\boxed{\vec{v}\times\vec{a}=(0,0,-2t\sin t-2\cos t)}.
$$

We can also factor out $$-2$$:

$$
\boxed{\vec{v}\times\vec{a}=(0,0,-2(t\sin t+\cos t))}.
$$

---

## 6. Geometric interpretation

The trajectory is

$$
\vec{r}(t)=(t^2,\sin t,5).
$$

Since the third coordinate is constant, the motion takes place entirely in the plane

$$
z=5.
$$

The velocity vector

$$
\vec{v}(t)=(2t,\cos t,0)
$$

is tangent to the trajectory, and the acceleration vector

$$
\vec{a}(t)=(2,-\sin t,0)
$$

describes how the velocity changes along the motion.

Because both vectors have zero third component, their cross product points in the $$z$$-direction, which is consistent with motion in a horizontal plane.

---

## Final answers

$$
\boxed{\vec{v}(t)=(2t,\cos t,0)}
$$

$$
\boxed{\vec{a}(t)=(2,-\sin t,0)}
$$

$$
\boxed{|\vec{v}(1)|=\sqrt{4+\cos^2 1}\approx2.07}
$$

$$
\boxed{\vec{v}\cdot\vec{a}=4t-\sin t\cos t}
$$

$$
\boxed{\vec{v}\times\vec{a}=(0,0,-2t\sin t-2\cos t)}
$$
