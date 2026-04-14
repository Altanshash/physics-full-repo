# Problem 9 – Harmonic oscillator

## Given

Consider the differential equation

$$
\frac{d^2x}{dt^2} + \omega^2 x = 0
$$

We need to:

1. find the general solution,
2. solve for the given initial conditions.

---

## 1. General solution

We solve the equation

$$
x'' + \omega^2 x = 0
$$

using the characteristic equation:

$$
r^2 + \omega^2 = 0
$$

So,

$$
r = \pm i\omega
$$

Therefore, the general solution is

$$
x(t) = C_1 \cos(\omega t) + C_2 \sin(\omega t)
$$

where $C_1$ and $C_2$ are constants.

---

## 2. Solution for initial conditions

Let the initial conditions be

$$
x(0) = x_0, \qquad x'(0) = v_0
$$

First compute the derivative:

$$
x'(t) = -C_1 \omega \sin(\omega t) + C_2 \omega \cos(\omega t)
$$

Now use the initial conditions.

### From $x(0)=x_0$

$$
x(0) = C_1 \cos 0 + C_2 \sin 0 = C_1
$$

So,

$$
C_1 = x_0
$$

### From $x'(0)=v_0$

$$
x'(0) = -C_1 \omega \sin 0 + C_2 \omega \cos 0 = C_2 \omega
$$

So,

$$
C_2 \omega = v_0
$$

$$
C_2 = \frac{v_0}{\omega}
$$

Therefore, the solution satisfying the initial conditions is

$$
x(t) = x_0 \cos(\omega t) + \frac{v_0}{\omega}\sin(\omega t)
$$

---

## Final answer

The general solution is

$$
x(t) = C_1 \cos(\omega t) + C_2 \sin(\omega t)
$$

If

$$
x(0)=x_0, \qquad x'(0)=v_0
$$

then the particular solution is

$$
x(t) = x_0 \cos(\omega t) + \frac{v_0}{\omega}\sin(\omega t)
$$
