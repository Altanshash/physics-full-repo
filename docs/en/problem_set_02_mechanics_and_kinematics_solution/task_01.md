## Problem 1 – Uniform and uniformly accelerated motion

### Problem statement

The equation of motion is

$$
x(t)=x_0+v_0t+\frac{1}{2}at^2
$$

Determine:

1. the velocity $v(t)$ and acceleration $a(t)$,
2. for $x_0=0$, $v_0=5\ \text{m/s}$, $a=-2\ \text{m/s}^2$:
   - the stopping time,
   - the maximum velocity depending on time and the sign of acceleration,
   - the maximum displacement,
3. visualize $x(t)$, $v(t)$, $a(t)$.

---

## Solution

### 1. Velocity and acceleration

The velocity is the derivative of position:

$$
v(t)=\frac{dx}{dt}
$$

Differentiate

$$
x(t)=x_0+v_0t+\frac{1}{2}at^2
$$

Then

$$
v(t)=v_0+at
$$

The acceleration is the derivative of velocity:

$$
a(t)=\frac{dv}{dt}
$$

So,

$$
a(t)=a
$$

Therefore,

$$
\boxed{v(t)=v_0+at}
$$

$$
\boxed{a(t)=a}
$$

---

### 2. Given values

We are given

$$
x_0=0,\qquad v_0=5,\qquad a=-2
$$

So the functions become

$$
x(t)=5t-\frac{1}{2}\cdot 2t^2
$$

Hence,

$$
x(t)=5t-t^2
$$

Velocity:

$$
v(t)=5-2t
$$

Acceleration:

$$
a(t)=-2
$$

---

### 3. Stopping time

The body stops when the velocity becomes zero:

$$
v(t)=0
$$

So,

$$
5-2t=0
$$

Thus,

$$
2t=5
$$

$$
t=\frac{5}{2}=2.5\ \text{s}
$$

Therefore,

$$
\boxed{t_{\text{stop}}=2.5\ \text{s}}
$$

---

### 4. Maximum velocity

Since

$$
v(t)=5-2t
$$

the velocity decreases with time because the acceleration is negative.

So the maximum velocity occurs at the initial moment:

$$
v_{\max}=v(0)=5\ \text{m/s}
$$

Therefore,

$$
\boxed{v_{\max}=5\ \text{m/s}}
$$

General interpretation:

- if $a<0$, velocity decreases with time,
- if $a=0$, velocity is constant,
- if $a>0$, velocity increases with time.

---

### 5. Maximum displacement

The maximum displacement is reached when the velocity becomes zero, that is at

$$
t=2.5\ \text{s}
$$

Now substitute this into the position function:

$$
x(t)=5t-t^2
$$

So,

$$
x(2.5)=5(2.5)-(2.5)^2
$$

$$
x(2.5)=12.5-6.25
$$

$$
x(2.5)=6.25\ \text{m}
$$

Therefore,

$$
\boxed{x_{\max}=6.25\ \text{m}}
$$

---

### 6. Visualization

The functions are

$$
x(t)=5t-t^2
$$

$$
v(t)=5-2t
$$

$$
a(t)=-2
$$

Their shapes are:

- $x(t)$ is a downward-opening parabola,
- $v(t)$ is a straight line with negative slope,
- $a(t)$ is a constant horizontal line.

---

## Conclusion

The velocity and acceleration are

$$
\boxed{v(t)=v_0+at}
$$

$$
\boxed{a(t)=a}
$$

For

$$
x_0=0,\qquad v_0=5,\qquad a=-2
$$

we obtain

$$
\boxed{x(t)=5t-t^2}
$$

$$
\boxed{v(t)=5-2t}
$$

$$
\boxed{a(t)=-2}
$$

The stopping time is

$$
\boxed{t_{\text{stop}}=2.5\ \text{s}}
$$

The maximum velocity is

$$
\boxed{v_{\max}=5\ \text{m/s}}
$$

The maximum displacement is

$$
\boxed{x_{\max}=6.25\ \text{m}}
$$
