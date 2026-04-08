## Problem 7 – Vertical throw with drag

### Problem statement

We consider the equation of motion

$$
m\frac{dv}{dt} = -mg - kv
$$

with initial conditions

$$
v(0)=v_0, \qquad x(0)=0
$$

Determine:

- the analytical solution,
- the maximum height,
- the comparison with the case without drag,
- a numerical simulation,
- the comparison between the analytical and numerical solutions.

---

## Solution

### 1. Equation for the velocity

Start from

$$
m\frac{dv}{dt} = -mg - kv
$$

Divide both sides by $m$:

$$
\frac{dv}{dt} + \frac{k}{m}v = -g
$$

This is a first-order linear differential equation.

---

### 2. Analytical solution for the velocity

The homogeneous equation is

$$
\frac{dv}{dt} + \frac{k}{m}v = 0
$$

Its solution is

$$
v_h(t)=Ce^{-kt/m}
$$

Now look for a constant particular solution $v_p$.  
If $v_p$ is constant, then $dv_p/dt=0$, so

$$
\frac{k}{m}v_p = -g
$$

Hence,

$$
v_p = -\frac{mg}{k}
$$

Therefore, the general solution is

$$
v(t)=Ce^{-kt/m}-\frac{mg}{k}
$$

Use the initial condition $v(0)=v_0$:

$$
v_0 = C - \frac{mg}{k}
$$

So,

$$
C = v_0 + \frac{mg}{k}
$$

Thus,

$$
v(t)=\left(v_0+\frac{mg}{k}\right)e^{-kt/m}-\frac{mg}{k}
$$

---

### 3. Position as a function of time

Since

$$
\frac{dx}{dt}=v(t),
$$

we integrate the velocity:

$$
x(t)=\int_0^t v(\tau)\,d\tau
$$

Substitute the velocity formula:

$$
x(t)=\int_0^t \left[\left(v_0+\frac{mg}{k}\right)e^{-k\tau/m}-\frac{mg}{k}\right] d\tau
$$

Split the integral:

$$
x(t)=\left(v_0+\frac{mg}{k}\right)\int_0^t e^{-k\tau/m}\,d\tau - \frac{mg}{k}\int_0^t d\tau
$$

Now compute the first integral:

$$
\int e^{-k\tau/m}\,d\tau = -\frac{m}{k}e^{-k\tau/m}
$$

So,

$$
\int_0^t e^{-k\tau/m}\,d\tau
=
\frac{m}{k}\left(1-e^{-kt/m}\right)
$$

Also,

$$
\int_0^t d\tau = t
$$

Therefore,

$$
x(t)=\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-kt/m}\right)-\frac{mg}{k}t
$$

This satisfies the initial condition $x(0)=0$.

---

### 4. Maximum height

The maximum height is reached when the velocity becomes zero:

$$
v(t_{\max})=0
$$

Using the velocity formula,

$$
\left(v_0+\frac{mg}{k}\right)e^{-kt_{\max}/m}-\frac{mg}{k}=0
$$

So,

$$
\left(v_0+\frac{mg}{k}\right)e^{-kt_{\max}/m}=\frac{mg}{k}
$$

Hence,

$$
e^{-kt_{\max}/m}=\frac{mg}{kv_0+mg}
$$

Take the logarithm:

$$
-\frac{k}{m}t_{\max}=\ln\left(\frac{mg}{kv_0+mg}\right)
$$

Therefore,

$$
t_{\max}=\frac{m}{k}\ln\left(\frac{kv_0+mg}{mg}\right)
$$

Now substitute this time into the position formula:

$$
x_{\max}=x(t_{\max})
$$

Using the expression above, we get

$$
x_{\max}
=
\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-kt_{\max}/m}\right)-\frac{mg}{k}t_{\max}
$$

Since

$$
e^{-kt_{\max}/m}=\frac{mg}{kv_0+mg},
$$

this simplifies to

$$
x_{\max}
=
\frac{mv_0}{k}
-
\frac{m^2g}{k^2}\ln\left(1+\frac{kv_0}{mg}\right)
$$

---

### 5. Comparison with motion without drag

Without drag, the equation becomes

$$
m\frac{dv}{dt}=-mg
$$

so

$$
\frac{dv}{dt}=-g
$$

With the initial condition $v(0)=v_0$, the solution is

$$
v(t)=v_0-gt
$$

Then the position is

$$
x(t)=v_0t-\frac{1}{2}gt^2
$$

The maximum height is reached when $v=0$:

$$
0=v_0-gt
$$

Thus,

$$
t_{\max}=\frac{v_0}{g}
$$

and

$$
x_{\max}=\frac{v_0^2}{2g}
$$

Therefore:

- without drag, the velocity decreases linearly,
- with drag, the velocity decreases faster because of the extra term $-kv$,
- with drag, the maximum height is smaller than in the drag-free case.

---

### 6. Numerical simulation

To simulate the motion numerically, use the system

$$
\frac{dx}{dt}=v
$$

$$
\frac{dv}{dt}=-g-\frac{k}{m}v
$$

Using the Euler method with time step $\Delta t$:

$$
v_{n+1}=v_n+\Delta t\left(-g-\frac{k}{m}v_n\right)
$$

$$
x_{n+1}=x_n+\Delta t\,v_n
$$

with initial values

$$
x_0=0, \qquad v_0=v_0
$$

This gives an approximate numerical solution step by step.

---

### 7. Analytical and numerical comparison

The analytical solution is

$$
v(t)=\left(v_0+\frac{mg}{k}\right)e^{-kt/m}-\frac{mg}{k}
$$

$$
x(t)=\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-kt/m}\right)-\frac{mg}{k}t
$$

The numerical solution approaches the same result when the time step $\Delta t$ is sufficiently small.

So:

- for small $\Delta t$, the agreement is very good,
- for larger $\Delta t$, the numerical error becomes more visible.

---

## Conclusion

The analytical velocity is

$$
v(t)=\left(v_0+\frac{mg}{k}\right)e^{-kt/m}-\frac{mg}{k}
$$

The analytical position is

$$
x(t)=\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-kt/m}\right)-\frac{mg}{k}t
$$

The time to the maximum height is

$$
t_{\max}=\frac{m}{k}\ln\left(\frac{kv_0+mg}{mg}\right)
$$

The maximum height is

$$
x_{\max}
=
\frac{mv_0}{k}
-
\frac{m^2g}{k^2}\ln\left(1+\frac{kv_0}{mg}\right)
$$

Compared with motion without drag, the body rises for a shorter time and reaches a lower maximum height.  
The numerical simulation confirms the analytical solution when the time step is small enough.
