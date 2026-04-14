# Problem 6 – Curve length and numerical integration

## Given

A parametric trajectory in 2D is

$$
x(t)=t, \qquad y(t)=t^2, \qquad t\in[0,1]
$$

We need to:

1. determine the velocity vector,
2. determine the magnitude of the velocity,
3. write the arc length as an integral,
4. compute the integral analytically if possible.

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
|\vec v(t)| = \sqrt{1+4t^2}
$$

---

## 3. Arc length integral

The arc length is

$$
s=\int_0^1 |\vec v(t)|\,dt
$$

So,

$$
s=\int_0^1 \sqrt{1+4t^2}\,dt
$$

---

## 4. Analytical calculation

Use the substitution

$$
u=2t, \qquad dt=\frac{du}{2}
$$

Then

$$
s=\frac12\int_0^2 \sqrt{1+u^2}\,du
$$

Using the standard formula

$$
\int \sqrt{1+u^2}\,du
=
\frac12\left(u\sqrt{1+u^2}+\ln\left|u+\sqrt{1+u^2}\right|\right)
$$

we get

$$
s
=
\frac14
\left[
u\sqrt{1+u^2}+\ln\left|u+\sqrt{1+u^2}\right|
\right]_0^2
$$

Therefore,

$$
s=\frac14\left(2\sqrt5+\ln(2+\sqrt5)\right)
$$

So,

$$
s=\frac{\sqrt5}{2}+\frac14\ln(2+\sqrt5)
$$

Approximate value:

$$
s \approx 1.47894
$$

---

## Final answers

$$
\vec v(t)=(1,2t)
$$

$$
|\vec v(t)|=\sqrt{1+4t^2}
$$

$$
s=\int_0^1 \sqrt{1+4t^2}\,dt
$$

$$
s=\frac{\sqrt5}{2}+\frac14\ln(2+\sqrt5)
$$

$$
s\approx1.47894
$$
