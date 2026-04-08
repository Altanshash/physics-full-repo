## Problem 6 – Motion with linear drag

### Problem statement

The drag force is given by

$$
F = -kv
$$

Initial conditions:

$$
v(0)=v_0, \qquad x(0)=0
$$

Determine:

- the equation of motion and its solution,
- the limit $\lim_{t\to\infty} v(t)$,
- the comparison with motion without drag.

---

## Solution

### 1. Equation of motion

Using Newton’s second law,

$$
m\frac{dv}{dt} = F
$$

and substituting the drag force, we obtain

$$
m\frac{dv}{dt} = -kv
$$

or

$$
\frac{dv}{dt} = -\frac{k}{m}v
$$

This is a separable differential equation.

---

### 2. Velocity as a function of time

Separate the variables:

$$
\frac{dv}{v} = -\frac{k}{m}\,dt
$$

Integrate both sides:

$$
\int \frac{dv}{v} = -\frac{k}{m}\int dt
$$

This gives

$$
\ln|v| = -\frac{k}{m}t + C
$$

Exponentiating:

$$
v(t) = Ce^{-kt/m}
$$

Now use the initial condition $v(0)=v_0$:

$$
v_0 = Ce^0 = C
$$

Hence,

$$
\boxed{v(t)=v_0e^{-kt/m}}
$$

So the velocity decreases exponentially with time.

---

### 3. Position as a function of time

Since

$$
\frac{dx}{dt}=v(t),
$$

we have

$$
\frac{dx}{dt}=v_0e^{-kt/m}
$$

Integrate from $0$ to $t$:

$$
x(t)-x(0)=\int_0^t v_0e^{-k\tau/m}\,d\tau
$$

Because $x(0)=0$, this becomes

$$
x(t)=v_0\int_0^t e^{-k\tau/m}\,d\tau
$$

Now compute the integral:

$$
\int e^{-k\tau/m}\,d\tau
=
-\frac{m}{k}e^{-k\tau/m}
$$

Therefore,

$$
x(t)
=
v_0
\left[
-\frac{m}{k}e^{-k\tau/m}
\right]_0^t
$$

Substitute the limits:

$$
x(t)
=
v_0
\left(
-\frac{m}{k}e^{-kt/m}
+\frac{m}{k}
\right)
$$

Thus,

$$
\boxed{
x(t)=\frac{mv_0}{k}\left(1-e^{-kt/m}\right)
}
$$

This satisfies the initial condition $x(0)=0$.

---

### 4. Limit of the velocity

From the velocity formula,

$$
v(t)=v_0e^{-kt/m}
$$

As $t\to\infty$,

$$
e^{-kt/m}\to 0
$$

Therefore,

$$
\boxed{
\lim_{t\to\infty} v(t)=0
}
$$

So the body gradually slows down and eventually comes to rest.

---

### 5. Comparison with motion without drag

If there is no drag, then

$$
F=0
$$

and Newton’s second law gives

$$
m\frac{dv}{dt}=0
$$

So the velocity remains constant:

$$
v(t)=v_0
$$

Then the position is

$$
x(t)=v_0t
$$

This is uniform motion.

With linear drag, the motion is different:

$$
v(t)=v_0e^{-kt/m}
$$

$$
x(t)=\frac{mv_0}{k}\left(1-e^{-kt/m}\right)
$$

Therefore:

- without drag, the speed stays constant,
- with drag, the speed decreases exponentially,
- without drag, the distance grows without bound,
- with drag, the position approaches a finite limit.

Indeed,

$$
\lim_{t\to\infty}x(t)=\frac{mv_0}{k}
$$

So in the presence of linear drag, the body travels only a finite total distance.

---

## Conclusion

The equation of motion is

$$
m\frac{dv}{dt}=-kv
$$

The velocity is

$$
\boxed{v(t)=v_0e^{-kt/m}}
$$

The position is

$$
\boxed{x(t)=\frac{mv_0}{k}\left(1-e^{-kt/m}\right)}
$$

Also,

$$
\boxed{\lim_{t\to\infty}v(t)=0}
$$

Thus, linear drag causes the body to slow down exponentially and eventually stop, unlike motion without drag, where the velocity remains constant.
