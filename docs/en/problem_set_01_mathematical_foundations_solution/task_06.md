# Problem 6 – Curve length and numerical integration

## Given

A parametric trajectory in 2D is given by

$$
x(t) = t, \qquad y(t) = t^2, \qquad t \in [0,1]
$$

Determine the velocity vector.

$$
\vec v(t) = \frac{d\vec r}{dt}
$$

Determine the magnitude of the velocity.

$$
|\vec v(t)|
$$

Write the arc length of the trajectory as an integral.

$$
s = \int_0^1 |\vec v(t)|\,dt
$$

Calculate this integral analytically if possible.

---

## 1. Velocity vector

The position vector is

$$
\vec r(t) = (t, t^2)
$$

Differentiate each component:

$$
\vec v(t) = \frac{d\vec r}{dt} = (1, 2t)
$$

---

## 2. Magnitude of the velocity

$$
|\vec v(t)| = \sqrt{1^2 + (2t)^2}
$$

$$
|\vec v(t)| = \sqrt{1 + 4t^2}
$$

---

## 3. Arc length integral

The arc length is

$$
s = \int_0^1 |\vec v(t)|\,dt
$$

Therefore,

$$
s = \int_0^1 \sqrt{1 + 4t^2}\,dt
$$

---

## 4. Analytical calculation

Use the substitution

$$
u = 2t, \qquad dt = \frac{du}{2}
$$

When $t=0$, we have $u=0$.  
When $t=1$, we have $u=2$.

So,

$$
s = \frac{1}{2}\int_0^2 \sqrt{1+u^2}\,du
$$

Use the standard formula

$$
\int \sqrt{1+u^2}\,du
=
\frac{1}{2}\left(u\sqrt{1+u^2} + \ln\left|u+\sqrt{1+u^2}\right|\right)
$$

Then

$$
s
=
\frac{1}{2}
\cdot
\frac{1}{2}
\left[
u\sqrt{1+u^2} + \ln\left|u+\sqrt{1+u^2}\right|
\right]_0^2
$$

So,

$$
s
=
\frac{1}{4}
\left[
u\sqrt{1+u^2} + \ln\left|u+\sqrt{1+u^2}\right|
\right]_0^2
$$

Evaluate at the bounds:

$$
s = \frac{1}{4}\left(2\sqrt{5} + \ln(2+\sqrt{5})\right)
$$

Therefore,

$$
s = \frac{\sqrt{5}}{2} + \frac{1}{4}\ln(2+\sqrt{5})
$$

Approximate value:

$$
s \approx 1.47894
$$

---

## Final answers

$$
\vec v(t) = (1, 2t)
$$

$$
|\vec v(t)| = \sqrt{1 + 4t^2}
$$

$$
s = \int_0^1 \sqrt{1 + 4t^2}\,dt
$$

$$
s = \frac{\sqrt{5}}{2} + \frac{1}{4}\ln(2+\sqrt{5})
$$

$$
s \approx 1.47894
$$
