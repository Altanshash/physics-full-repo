## Problem 3 – Elimination of time and interpretation of acceleration

### Given

$$
x(t)=2t^2,\qquad y(t)=3t^3
$$

### 1. Eliminate the parameter $t$

From

$$
x=2t^2
$$

we get

$$
t^2=\frac{x}{2}.
$$

Also,

$$
y=3t^3.
$$

Squaring both sides:

$$
y^2=9t^6.
$$

Since

$$
t^6=(t^2)^3=\left(\frac{x}{2}\right)^3=\frac{x^3}{8},
$$

then

$$
y^2=9\cdot\frac{x^3}{8}=\frac{9}{8}x^3.
$$

Therefore,

$$
\boxed{y^2=\frac{9}{8}x^3}, \qquad x\ge 0
$$

### 2. Trajectory

The trajectory is given by

$$
y^2=\frac{9}{8}x^3, \qquad x\ge 0.
$$

This is a **semicubical parabola** opening to the right.

- At $t=0$, the particle is at the point $(0,0)$.
- For $t>0$, the motion is along the upper branch.
- For $t<0$, the motion is along the lower branch.

### 3. Find $\vec{v}(t)$, $|\vec{v}(t)|$, $\vec{a}(t)$, and $|\vec{a}(t)|$

The velocity vector is

$$
\vec{v}(t)=\left(\frac{dx}{dt},\frac{dy}{dt}\right).
$$

Since

$$
\frac{dx}{dt}=4t,\qquad \frac{dy}{dt}=9t^2,
$$

we obtain

$$
\boxed{\vec{v}(t)=(4t,\,9t^2)}.
$$

Its magnitude is

$$
|\vec{v}(t)|=\sqrt{(4t)^2+(9t^2)^2}
=\sqrt{16t^2+81t^4}.
$$

Thus,

$$
\boxed{|\vec{v}(t)|=\sqrt{16t^2+81t^4}}.
$$

The acceleration vector is

$$
\vec{a}(t)=\left(\frac{d^2x}{dt^2},\frac{d^2y}{dt^2}\right).
$$

Since

$$
\frac{d^2x}{dt^2}=4,\qquad \frac{d^2y}{dt^2}=18t,
$$

we get

$$
\boxed{\vec{a}(t)=(4,\,18t)}.
$$

Its magnitude is

$$
|\vec{a}(t)|=\sqrt{4^2+(18t)^2}
=\sqrt{16+324t^2}.
$$

Hence,

$$
\boxed{|\vec{a}(t)|=\sqrt{16+324t^2}}.
$$

### 4. Is the acceleration constant?

Since

$$
\vec{a}(t)=(4,18t),
$$

the second component depends on $t$. Therefore, the acceleration is **not constant**.

$$
\boxed{\text{The acceleration is not constant.}}
$$
