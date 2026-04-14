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

#### 1. Velocity vector

Since acceleration is constant,

$$
\vec{a}(t)=\frac{d\vec{v}}{dt}=(2,-3).
$$

Integrating with respect to time, we obtain

$$
\vec{v}(t)=(2t+C_1,\,-3t+C_2).
$$

Using the initial condition

$$
\vec{v}(0)=(1,0),
$$

we find

$$
C_1=1, \qquad C_2=0.
$$

Therefore,

$$
\boxed{\vec{v}(t)=(2t+1,\,-3t)}.
$$

---

#### 2. Position vector

Now

$$
\frac{d\vec{r}}{dt}=\vec{v}(t)=(2t+1,\,-3t).
$$

Integrating again, we get

$$
\vec{r}(t)=\left(t^2+t+C_3,\,-\frac{3}{2}t^2+C_4\right).
$$

Using the initial condition

$$
\vec{r}(0)=(0,0),
$$

we obtain

$$
C_3=0, \qquad C_4=0.
$$

Hence,

$$
\boxed{\vec{r}(t)=\left(t^2+t,\,-\frac{3}{2}t^2\right)}.
$$

---

#### 3. Trajectory equation

From the position vector,

$$
x=t^2+t,
\qquad
y=-\frac{3}{2}t^2.
$$

From the second equation,

$$
t^2=-\frac{2}{3}y.
$$

Using the first equation,

$$
x=t^2+t.
$$

Substitute $t^2=-\dfrac{2}{3}y$:

$$
x=-\frac{2}{3}y+t.
$$

So,

$$
t=x+\frac{2}{3}y.
$$

Now square both sides:

$$
t^2=\left(x+\frac{2}{3}y\right)^2.
$$

But since

$$
t^2=-\frac{2}{3}y,
$$

we get

$$
\left(x+\frac{2}{3}y\right)^2=-\frac{2}{3}y.
$$

Therefore, the trajectory is

$$
\boxed{\left(x+\frac{2}{3}y\right)^2=-\frac{2}{3}y}.
$$

This is a parabola.

---

#### 4. Selected moments

At $t=0$:

$$
\vec{r}(0)=(0,0), \qquad \vec{v}(0)=(1,0), \qquad \vec{a}=(2,-3).
$$

At $t=1$:

$$
\vec{r}(1)=\left(1^2+1,\,-\frac{3}{2}\cdot1^2\right)=\left(2,-\frac{3}{2}\right),
$$

$$
\vec{v}(1)=(2\cdot1+1,\,-3\cdot1)=(3,-3),
$$

$$
\vec{a}=(2,-3).
$$

At $t=2$:

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

#### 5. Interpretation of the motion

The body starts at the origin:

$$
\vec{r}(0)=(0,0).
$$

Its initial velocity is horizontal:

$$
\vec{v}(0)=(1,0).
$$

The acceleration is constant:

$$
\vec{a}=(2,-3).
$$

Thus, the horizontal component of velocity increases linearly with time, while the vertical component decreases linearly with time.

As a result, the body moves along a parabolic trajectory in the plane.

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

Therefore, this is a two-dimensional motion with constant acceleration, linear change of velocity, and a parabolic trajectory.
