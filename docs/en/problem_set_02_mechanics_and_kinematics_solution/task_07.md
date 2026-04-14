## Problem 7 – 2D motion with a given acceleration

### Given

The acceleration is

$$
\vec{a}=(2,-3)
$$

and the initial conditions are

$$
\vec{v}(0)=(1,0), \qquad \vec{r}(0)=(0,0).
$$

Find:

1. Determine $\vec{v}(t)$
2. Determine $\vec{r}(t)$
3. Draw the trajectory, velocity vector, and acceleration vector at a few selected moments in time

---

### Solution

#### 1. Acceleration

The acceleration is constant:

$$
\vec{a}(t)=(2,-3).
$$

This means that

$$
\frac{d\vec{v}}{dt}=\vec{a}=(2,-3).
$$

---

#### 2. Velocity vector

To find the velocity vector, integrate the acceleration with respect to time:

$$
\vec{v}(t)=\int \vec{a}\,dt=(2t+C_1,\,-3t+C_2).
$$

Now use the initial condition

$$
\vec{v}(0)=(1,0).
$$

Substituting $t=0$, we get

$$
(C_1,C_2)=(1,0).
$$

Therefore,

$$
\boxed{\vec{v}(t)=(2t+1,\,-3t)}.
$$

---

#### 3. Position vector

The position vector satisfies

$$
\frac{d\vec{r}}{dt}=\vec{v}(t)=(2t+1,\,-3t).
$$

Integrate each component:

$$
\vec{r}(t)=\int \vec{v}(t)\,dt=(t^2+t+C_3,\,-\frac{3}{2}t^2+C_4).
$$

Now use the initial condition

$$
\vec{r}(0)=(0,0).
$$

Substituting $t=0$, we obtain

$$
(C_3,C_4)=(0,0).
$$

Hence,

$$
\boxed{\vec{r}(t)=\left(t^2+t,\,-\frac{3}{2}t^2\right)}.
$$

---

#### 4. Trajectory equation

From the position vector,

$$
x=t^2+t,
\qquad
y=-\frac{3}{2}t^2.
$$

To describe the trajectory, we eliminate the parameter $t$.

From

$$
y=-\frac{3}{2}t^2,
$$

we get

$$
t^2=-\frac{2}{3}y.
$$

Using

$$
x=t^2+t,
$$

we can also write

$$
t=x-t^2=x+\frac{2}{3}y.
$$

A simpler way is to solve for $t$ from the first relation:

$$
t^2=-\frac{2}{3}y.
$$

Then from

$$
x=t^2+t,
$$

we get

$$
t=x+\frac{2}{3}y.
$$

Squaring this expression:

$$
\left(x+\frac{2}{3}y\right)^2=t^2.
$$

But since

$$
t^2=-\frac{2}{3}y,
$$

we finally obtain

$$
\left(x+\frac{2}{3}y\right)^2=-\frac{2}{3}y.
$$

Therefore, the trajectory equation is

$$
\boxed{\left(x+\frac{2}{3}y\right)^2=-\frac{2}{3}y}.
$$

This is a parabola.

---

#### 5. Selected moments

##### At $t=0$

$$
\vec{r}(0)=(0,0), \qquad \vec{v}(0)=(1,0), \qquad \vec{a}=(2,-3).
$$

##### At $t=1$

$$
\vec{r}(1)=\left(1^2+1,\,-\frac{3}{2}\cdot1^2\right)=\left(2,-\frac{3}{2}\right),
$$

$$
\vec{v}(1)=(2\cdot1+1,\,-3\cdot1)=(3,-3),
$$

$$
\vec{a}=(2,-3).
$$

##### At $t=2$

$$
\vec{r}(2)=\left(2^2+2,\,-\frac{3}{2}\cdot2^2\right)=(6,-6),
$$

$$
\vec{v}(2)=(2\cdot2+1,\,-3\cdot2)=(5,-6),
$$

$$
\vec{a}=(2,-3).
$$

These points can be used to sketch the trajectory and the vectors.

---

#### 6. Interpretation of the motion

- The body starts at the origin:
  $$
  \vec{r}(0)=(0,0)
  $$
- Its initial velocity is horizontal:
  $$
  \vec{v}(0)=(1,0)
  $$
- The acceleration is constant:
  $$
  \vec{a}=(2,-3)
  $$

So:

- the $x$-component of velocity increases linearly because of the positive acceleration $2$
- the $y$-component of velocity decreases linearly because of the negative acceleration $-3$

As a result, the body moves along a **parabolic trajectory** in the plane.

---

### Final Conclusion

For the constant acceleration

$$
\vec{a}=(2,-3),
$$

with initial conditions

$$
\vec{v}(0)=(1,0), \qquad \vec{r}(0)=(0,0),
$$

the velocity vector is

$$
\boxed{\vec{v}(t)=(2t+1,\,-3t)}
$$

and the position vector is

$$
\boxed{\vec{r}(t)=\left(t^2+t,\,-\frac{3}{2}t^2\right)}.
$$

The trajectory is the parabola

$$
\boxed{\left(x+\frac{2}{3}y\right)^2=-\frac{2}{3}y}.
$$

Thus, the motion is a two-dimensional motion with constant acceleration, where the velocity changes linearly with time and the position follows a parabolic path.
