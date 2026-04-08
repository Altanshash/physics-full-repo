## Problem 7 – Vertical throw with drag

### Problem statement

We consider the equation of motion

$$
m \frac{dv}{dt} = -mg - kv
$$

with initial conditions

$$
v(0) = v_0, \qquad x(0) = 0
$$

Determine:

- the analytical solution,
- the maximum height,
- comparison with motion without drag,
- numerical simulation,
- comparison of analytical and numerical results.

---

## Solution

### 1. Equation for the velocity

Starting from

$$
m \frac{dv}{dt} = -mg - kv
$$

divide by $m$:

$$
\frac{dv}{dt} + \frac{k}{m} v = -g
$$

---

### 2. Velocity solution

Solve the homogeneous equation:

$$
\frac{dv}{dt} + \frac{k}{m} v = 0
$$

$$
v_h(t) = C e^{-kt/m}
$$

Particular solution:

$$
\frac{k}{m} v_p = -g
\quad \Rightarrow \quad
v_p = -\frac{mg}{k}
$$

General solution:

$$
v(t) = C e^{-kt/m} - \frac{mg}{k}
$$

Apply initial condition:

$$
v(0) = v_0 = C - \frac{mg}{k}
$$

$$
C = v_0 + \frac{mg}{k}
$$

Final velocity:

$$
v(t) = \left(v_0 + \frac{mg}{k}\right) e^{-kt/m} - \frac{mg}{k}
$$

---

### 3. Position function

$$
\frac{dx}{dt} = v(t)
$$

$$
x(t) = \int_0^t v(\tau)\, d\tau
$$

$$
x(t) =
\int_0^t
\left[
\left(v_0 + \frac{mg}{k}\right) e^{-k\tau/m}
-
\frac{mg}{k}
\right]
d\tau
$$

Compute integrals:

$$
\int_0^t e^{-k\tau/m} d\tau =
\frac{m}{k}\left(1 - e^{-kt/m}\right)
$$

$$
\int_0^t d\tau = t
$$

Final position:

$$
x(t) =
\frac{m}{k}
\left(v_0 + \frac{mg}{k}\right)
\left(1 - e^{-kt/m}\right)
-
\frac{mg}{k} t
$$

---

### 4. Maximum height

Condition:

$$
v(t_{\max}) = 0
$$

$$
\left(v_0 + \frac{mg}{k}\right)e^{-kt_{\max}/m}
=
\frac{mg}{k}
$$

$$
e^{-kt_{\max}/m}
=
\frac{mg}{kv_0 + mg}
$$

$$
t_{\max}
=
\frac{m}{k}
\ln\left(\frac{kv_0 + mg}{mg}\right)
$$

Maximum height:

$$
x_{\max} =
\frac{mv_0}{k}
-
\frac{m^2 g}{k^2}
\ln\left(1 + \frac{k v_0}{mg}\right)
$$

---

### 5. Without drag

$$
\frac{dv}{dt} = -g
$$

$$
v(t) = v_0 - gt
$$

$$
x(t) = v_0 t - \frac{1}{2} g t^2
$$

$$
t_{\max} = \frac{v_0}{g}
$$

$$
x_{\max} = \frac{v_0^2}{2g}
$$

---

### 6. Numerical method

$$
\frac{dx}{dt} = v
$$

$$
\frac{dv}{dt} = -g - \frac{k}{m}v
$$

Euler method:

$$
v_{n+1} = v_n + \Delta t \left(-g - \frac{k}{m} v_n \right)
$$

$$
x_{n+1} = x_n + \Delta t \, v_n
$$

---

## Conclusion

$$
v(t) =
\left(v_0 + \frac{mg}{k}\right)e^{-kt/m} - \frac{mg}{k}
$$

$$
x(t) =
\frac{m}{k}
\left(v_0 + \frac{mg}{k}\right)
\left(1 - e^{-kt/m}\right)
-
\frac{mg}{k} t
$$

$$
t_{\max} =
\frac{m}{k}
\ln\left(\frac{kv_0 + mg}{mg}\right)
$$

$$
x_{\max} =
\frac{mv_0}{k}
-
\frac{m^2 g}{k^2}
\ln\left(1 + \frac{k v_0}{mg}\right)
$$
