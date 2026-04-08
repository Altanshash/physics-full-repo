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

and substituting the drag force $F=-kv$, we get

$$
m\frac{dv}{dt} = -kv
$$

or equivalently,

$$
\frac{dv}{dt} = -\frac{k}{m}v
$$

This is a first-order differential equation with separable variables.

---

### 2. Solution for the velocity

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
\ln |v| = -\frac{k}{m}t + C
$$

Exponentiating both sides, we obtain

$$
v(t) = Ce^{-kt/m}
$$

Now apply the initial condition $v(0)=v_0$:

$$
v_0 = Ce^0 = C
$$

Hence,

$$
\boxed{
v(t)=v_0e^{-kt/m}
}
$$

So the velocity decreases exponentially with time.

---

### 3. Solution for the position

Since velocity is the derivative of position,

$$
\frac{dx}{dt}=v(t)=v_0e^{-kt/m}
$$

Integrate from $0$ to $t$:

$$
x(t)=\int_0^t v_0e^{-k\tau/m}\,d\tau
$$

Take $v_0$ outside the integral:

$$
x(t)=v_0\int_0^t e^{-k\tau/m}\,d\tau
$$

Now integrate:

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

So,

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

If there is no drag, then the force is zero:

$$
F=0
$$

Hence, Newton’s second law gives

$$
m\frac{dv}{dt}=0
$$

which means

$$
v(t)=v_0
$$

So without drag, the velocity remains constant and the motion is uniform:

$$
x(t)=v_0t
$$

With linear drag, the motion is different:

$$
v(t)=v_0e^{-kt/m}
$$

$$
x(t)=\frac{mv_0}{k}\left(1-e^{-kt/m}\right)
$$

Thus:

- without drag, the body moves forever with constant speed,
- with drag, the speed decreases exponentially,
- with drag, the position approaches the finite limit

$$
\lim_{t\to\infty}x(t)=\frac{mv_0}{k}
$$

So in the presence of linear drag, the body travels only a finite distance.

---

## Conclusion

The equation of motion is

$$
m\frac{dv}{dt}=-kv
$$

Its solution for velocity is

$$
\boxed{
v(t)=v_0e^{-kt/m}
}
$$

The position is

$$
\boxed{
x(t)=\frac{mv_0}{k}\left(1-e^{-kt/m}\right)
}
$$

Also,

$$
\boxed{
\lim_{t\to\infty}v(t)=0
}
$$

Compared with motion without drag, linear resistance causes the velocity to decay exponentially and limits the total distance traveled.
