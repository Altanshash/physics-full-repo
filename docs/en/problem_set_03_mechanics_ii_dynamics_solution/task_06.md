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

- the equation of motion and solve it,
- the limit $\lim_{t\to\infty} v(t)$,
- compare the result with motion without drag.

---

## Solution

### 1. Equation of motion

Using Newton’s second law,

$$
m\frac{dv}{dt} = F
$$

Substitute the drag force:

$$
m\frac{dv}{dt} = -kv
$$

So the equation of motion is

$$
\frac{dv}{dt} = -\frac{k}{m}v
$$

This is a first-order separable differential equation.

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
\ln |v| = -\frac{k}{m}t + C
$$

Exponentiating, we obtain

$$
v(t) = Ce^{-kt/m}
$$

Now apply the initial condition $v(0)=v_0$:

$$
v_0 = Ce^0 = C
$$

Therefore,

$$
v(t) = v_0e^{-kt/m}
$$

So the velocity decreases exponentially with time.

---

### 3. Position as a function of time

Since

$$
\frac{dx}{dt} = v(t)
$$

we have

$$
\frac{dx}{dt} = v_0e^{-kt/m}
$$

Integrate from $0$ to $t$:

$$
x(t) = \int_0^t v_0e^{-k\tau/m}\,d\tau
$$

Take $v_0$ outside the integral:

$$
x(t) = v_0 \int_0^t e^{-k\tau/m}\,d\tau
$$

Now integrate:

$$
\int e^{-k\tau/m}\,d\tau = -\frac{m}{k}e^{-k\tau/m}
$$

So,

$$
x(t) = v_0 \left[ -\frac{m}{k}e^{-k\tau/m} \right]_0^t
$$

Substitute the limits:

$$
x(t) = v_0 \left( -\frac{m}{k}e^{-kt/m} + \frac{m}{k} \right)
$$

Hence,

$$
x(t) = \frac{mv_0}{k}\left(1-e^{-kt/m}\right)
$$

This satisfies the initial condition $x(0)=0$.

---

### 4. Limit of the velocity

From the velocity formula,

$$
v(t) = v_0e^{-kt/m}
$$

As $t \to \infty$,

$$
e^{-kt/m} \to 0
$$

Therefore,

$$
\lim_{t\to\infty} v(t) = 0
$$

So the body gradually slows down and eventually stops.

---

### 5. Comparison with motion without drag

If there is no drag, then

$$
F = 0
$$

and Newton’s second law becomes

$$
m\frac{dv}{dt} = 0
$$

Hence,

$$
v(t) = v_0
$$

So the velocity remains constant.

The position is then

$$
x(t) = v_0 t
$$

This is uniform motion.

With linear drag, we found

$$
v(t) = v_0e^{-kt/m}
$$

and

$$
x(t) = \frac{mv_0}{k}\left(1-e^{-kt/m}\right)
$$

Therefore:

- without drag, the body moves with constant velocity,
- with drag, the velocity decreases exponentially,
- without drag, the distance keeps increasing,
- with drag, the position approaches a finite limit.

Indeed,

$$
\lim_{t\to\infty} x(t) = \frac{mv_0}{k}
$$

So with linear drag, the body travels only a finite total distance.

---

## Conclusion

The equation of motion is

$$
m\frac{dv}{dt} = -kv
$$

The velocity is

$$
v(t) = v_0e^{-kt/m}
$$

The position is

$$
x(t) = \frac{mv_0}{k}\left(1-e^{-kt/m}\right)
$$

Also,

$$
\lim_{t\to\infty} v(t) = 0
$$

Thus, linear drag causes the body to slow down exponentially and eventually stop, unlike motion without drag, where the velocity remains constant.
