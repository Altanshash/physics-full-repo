## Problem 7 – Vertical throw with drag

### Problem statement

We consider the equation of motion

$$
m \frac{dv}{dt} = -mg - kv
$$

with initial conditions

$$
v(0)=v_0, \qquad x(0)=0
$$

Determine:

- solve the equation,
- determine the maximum height,
- compare with the case without drag,
- perform a numerical simulation,
- compare the analytical and numerical solutions.

---

## Solution

### 1. Differential equation for velocity

Starting from

$$
m \frac{dv}{dt} = -mg - kv
$$

divide both sides by $m$:

$$
\frac{dv}{dt} + \frac{k}{m}v = -g
$$

This is a first-order linear differential equation.

---

### 2. Velocity function

First solve the homogeneous equation:

$$
\frac{dv}{dt} + \frac{k}{m}v = 0
$$

Its solution is

$$
v_h(t)=Ce^{-kt/m}
$$

Now find a constant particular solution $v_p$.

If $v_p$ is constant, then

$$
\frac{dv_p}{dt}=0
$$

so the equation becomes

$$
\frac{k}{m}v_p=-g
$$

Hence,

$$
v_p=-\frac{mg}{k}
$$

Therefore, the general solution is

$$
v(t)=Ce^{-kt/m}-\frac{mg}{k}
$$

Apply the initial condition $v(0)=v_0$:

$$
v_0=C-\frac{mg}{k}
$$

Thus,

$$
C=v_0+\frac{mg}{k}
$$

So the velocity is

$$
\boxed{
v(t)=\left(v_0+\frac{mg}{k}\right)e^{-kt/m}-\frac{mg}{k}
}
$$

---

### 3. Position function

Since

$$
\frac{dx}{dt}=v(t)
$$

we integrate:

$$
x(t)=\int_0^t v(\tau)\,d\tau
$$

Substitute the velocity:

$$
x(t)=\int_0^t \left[\left(v_0+\frac{mg}{k}\right)e^{-k\tau/m}-\frac{mg}{k}\right] d\tau
$$

Split the integral:

$$
x(t)=\left(v_0+\frac{mg}{k}\right)\int_0^t e^{-k\tau/m}d\tau-\frac{mg}{k}\int_0^t d\tau
$$

Now compute the two integrals:

$$
\int_0^t e^{-k\tau/m}d\tau=\frac{m}{k}\left(1-e^{-kt/m}\right)
$$

and

$$
\int_0^t d\tau=t
$$

Therefore,

$$
\boxed{
x(t)=\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-kt/m}\right)-\frac{mg}{k}t
}
$$

This satisfies $x(0)=0$.

---

### 4. Maximum height

The maximum height is reached when the velocity becomes zero:

$$
v(t_{\max})=0
$$

Using the velocity formula:

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

Take the natural logarithm:

$$
-\frac{k}{m}t_{\max}=\ln\left(\frac{mg}{kv_0+mg}\right)
$$

Therefore,

$$
\boxed{
t_{\max}=\frac{m}{k}\ln\left(\frac{kv_0+mg}{mg}\right)
}
$$

Now substitute this time into the position formula. The maximum height is

$$
x_{\max}=x(t_{\max})
$$

After simplification, we obtain

$$
\boxed{
x_{\max}=\frac{mv_0}{k}-\frac{m^2g}{k^2}\ln\left(1+\frac{kv_0}{mg}\right)
}
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

With $v(0)=v_0$, the velocity is

$$
v(t)=v_0-gt
$$

and the position is

$$
x(t)=v_0t-\frac{1}{2}gt^2
$$

The maximum height is reached when $v=0$:

$$
t_{\max}=\frac{v_0}{g}
$$

and

$$
x_{\max}=\frac{v_0^2}{2g}
$$

So:

- without drag, the body rises higher,
- with drag, the body slows down faster,
- with drag, the maximum height is smaller.

---

### 6. Numerical simulation

The motion can also be simulated numerically using the system

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

### 7. Comparison of analytical and numerical solutions

The analytical solution is

$$
v(t)=\left(v_0+\frac{mg}{k}\right)e^{-kt/m}-\frac{mg}{k}
$$

$$
x(t)=\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-kt/m}\right)-\frac{mg}{k}t
$$

The numerical solution approaches the same result when the time step is sufficiently small.

Thus:

- for small $\Delta t$, the agreement is good,
- for large $\Delta t$, the numerical error becomes more noticeable.

---

## Conclusion

The velocity is

$$
\boxed{
v(t)=\left(v_0+\frac{mg}{k}\right)e^{-kt/m}-\frac{mg}{k}
}
$$

The position is

$$
\boxed{
x(t)=\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-kt/m}\right)-\frac{mg}{k}t
}
$$

The time to the maximum height is

$$
\boxed{
t_{\max}=\frac{m}{k}\ln\left(\frac{kv_0+mg}{mg}\right)
}
$$

The maximum height is

$$
\boxed{
x_{\max}=\frac{mv_0}{k}-\frac{m^2g}{k^2}\ln\left(1+\frac{kv_0}{mg}\right)
}
$$
