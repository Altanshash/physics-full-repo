## Problem 7 – Vertical throw with drag

### Problem statement

We consider the equation of motion

$m \dfrac{dv}{dt} = -mg - kv$

with initial conditions

$v(0)=v_0$, $x(0)=0$.

Determine:

- the analytical solution,
- the maximum height,
- the comparison with the case without drag,
- a numerical simulation,
- the comparison between the analytical and numerical solutions.

---

## Solution

### 1. Equation for the velocity

Starting from

$m \dfrac{dv}{dt} = -mg - kv$

divide both sides by $m$:

$\dfrac{dv}{dt} + \dfrac{k}{m}v = -g$

This is a first-order linear differential equation.

---

### 2. Analytical solution for the velocity

First solve the homogeneous equation:

$\dfrac{dv}{dt} + \dfrac{k}{m}v = 0$

Its solution is

$v_h(t)=Ce^{-kt/m}$

Now look for a constant particular solution $v_p$.  
If $v_p$ is constant, then $dv_p/dt=0$, so

$\dfrac{k}{m}v_p=-g$

Hence,

$v_p=-\dfrac{mg}{k}$

So the general solution is

$v(t)=Ce^{-kt/m}-\dfrac{mg}{k}$

Apply the initial condition $v(0)=v_0$:

$v_0=C-\dfrac{mg}{k}$

Therefore,

$C=v_0+\dfrac{mg}{k}$

Thus, the velocity is

$v(t)=\left(v_0+\dfrac{mg}{k}\right)e^{-kt/m}-\dfrac{mg}{k}$

---

### 3. Position as a function of time

Since

$\dfrac{dx}{dt}=v(t)$

we integrate the velocity:

$x(t)=\int_0^t v(\tau)\,d\tau$

Substitute the formula for velocity:

$x(t)=\int_0^t \left[\left(v_0+\dfrac{mg}{k}\right)e^{-k\tau/m}-\dfrac{mg}{k}\right]d\tau$

Split the integral:

$x(t)=\left(v_0+\dfrac{mg}{k}\right)\int_0^t e^{-k\tau/m}d\tau-\dfrac{mg}{k}\int_0^t d\tau$

Now compute the integrals:

$\int_0^t e^{-k\tau/m}d\tau=\dfrac{m}{k}\left(1-e^{-kt/m}\right)$

and

$\int_0^t d\tau=t$

So we get

$x(t)=\dfrac{m}{k}\left(v_0+\dfrac{mg}{k}\right)\left(1-e^{-kt/m}\right)-\dfrac{mg}{k}t$

This also satisfies $x(0)=0$.

---

### 4. Maximum height

The maximum height is reached when the velocity becomes zero:

$v(t_{\max})=0$

Using the velocity formula,

$\left(v_0+\dfrac{mg}{k}\right)e^{-kt_{\max}/m}-\dfrac{mg}{k}=0$

So,

$\left(v_0+\dfrac{mg}{k}\right)e^{-kt_{\max}/m}=\dfrac{mg}{k}$

Hence,

$e^{-kt_{\max}/m}=\dfrac{mg}{kv_0+mg}$

Take the natural logarithm:

$-\dfrac{k}{m}t_{\max}=\ln\left(\dfrac{mg}{kv_0+mg}\right)$

Therefore,

$t_{\max}=\dfrac{m}{k}\ln\left(\dfrac{kv_0+mg}{mg}\right)$

Now substitute this into the position formula:

$x_{\max}=x(t_{\max})$

So,

$x_{\max}=\dfrac{m}{k}\left(v_0+\dfrac{mg}{k}\right)\left(1-e^{-kt_{\max}/m}\right)-\dfrac{mg}{k}t_{\max}$

Using

$e^{-kt_{\max}/m}=\dfrac{mg}{kv_0+mg}$

this simplifies to

$x_{\max}=\dfrac{mv_0}{k}-\dfrac{m^2g}{k^2}\ln\left(1+\dfrac{kv_0}{mg}\right)$

---

### 5. Comparison with motion without drag

Without drag, the equation becomes

$m\dfrac{dv}{dt}=-mg$

so

$\dfrac{dv}{dt}=-g$

With the initial condition $v(0)=v_0$, the velocity is

$v(t)=v_0-gt$

and the position is

$x(t)=v_0t-\dfrac{1}{2}gt^2$

The maximum height is reached when $v=0$, so

$t_{\max}=\dfrac{v_0}{g}$

and

$x_{\max}=\dfrac{v_0^2}{2g}$

Therefore:

- without drag, the velocity decreases linearly,
- with drag, the velocity decreases faster,
- with drag, the body reaches a smaller maximum height.

---

### 6. Numerical simulation

To simulate the motion numerically, use the system

$\dfrac{dx}{dt}=v$

$\dfrac{dv}{dt}=-g-\dfrac{k}{m}v$

Using the Euler method with time step $\Delta t$:

$v_{n+1}=v_n+\Delta t\left(-g-\dfrac{k}{m}v_n\right)$

$x_{n+1}=x_n+\Delta t\,v_n$

with initial values

$x_0=0$, $v_0=v_0$

This gives an approximate solution step by step.

---

### 7. Comparison of analytical and numerical solutions

The analytical solution is

$v(t)=\left(v_0+\dfrac{mg}{k}\right)e^{-kt/m}-\dfrac{mg}{k}$

$x(t)=\dfrac{m}{k}\left(v_0+\dfrac{mg}{k}\right)\left(1-e^{-kt/m}\right)-\dfrac{mg}{k}t$

The numerical solution approaches the same result when the time step $\Delta t$ is sufficiently small.

So:

- for small $\Delta t$, the agreement is very good,
- for large $\Delta t$, the numerical error becomes noticeable.

---

## Conclusion

The velocity is

$v(t)=\left(v_0+\dfrac{mg}{k}\right)e^{-kt/m}-\dfrac{mg}{k}$

The position is

$x(t)=\dfrac{m}{k}\left(v_0+\dfrac{mg}{k}\right)\left(1-e^{-kt/m}\right)-\dfrac{mg}{k}t$

The time to the maximum height is

$t_{\max}=\dfrac{m}{k}\ln\left(\dfrac{kv_0+mg}{mg}\right)$

The maximum height is

$x_{\max}=\dfrac{mv_0}{k}-\dfrac{m^2g}{k^2}\ln\left(1+\dfrac{kv_0}{mg}\right)$

Compared with motion without drag, the body rises for a shorter time and reaches a lower maximum height.  
The numerical simulation agrees with the analytical solution when the time step is small enough.
