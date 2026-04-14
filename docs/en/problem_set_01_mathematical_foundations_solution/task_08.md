# Problem 8 – First-order differential equation

## Given

Consider the differential equation

$$
\frac{dy}{dt} = -ky
$$

We need to solve the equation.

---

## 1. Solve the equation

We use separation of variables:

$$
\frac{dy}{dt} = -ky
$$

Rewrite it as

$$
\frac{dy}{y} = -k\,dt
$$

Now integrate both sides:

$$
\int \frac{1}{y}\,dy = \int -k\,dt
$$

This gives

$$
\ln|y| = -kt + C
$$

where $C$ is the constant of integration.

Now exponentiate both sides:

$$
|y| = e^{-kt+C}
$$

We can write $e^C$ as a new constant $C_1>0$, so

$$
|y| = C_1 e^{-kt}
$$

Thus the general solution can be written as

$$
y(t) = C e^{-kt}
$$

where $C$ is an arbitrary constant.

---

## 2. Solution with initial condition

If the initial condition is

$$
y(0)=y_0
$$

then substitute $t=0$ into the general solution:

$$
y(0)=Ce^{0}=C
$$

So,

$$
C=y_0
$$

Therefore, the solution satisfying the initial condition is

$$
y(t)=y_0 e^{-kt}
$$

---

## Final answer

The general solution is

$$
y(t)=Ce^{-kt}
$$

If

$$
y(0)=y_0
$$

then the particular solution is

$$
y(t)=y_0 e^{-kt}
$$
