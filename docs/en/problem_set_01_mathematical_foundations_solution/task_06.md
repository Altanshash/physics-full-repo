# Problem 6 – Curve length and numerical integration

## Given

A parametric trajectory in 2D is given by

$$
x(t) = t, \qquad y(t) = t^2, \qquad t \in [0,1]
$$

Determine:

1. the velocity vector
2. the magnitude of the velocity
3. the arc length as an integral
4. evaluate the integral analytically

---

## 1. Velocity vector

The position vector is

$$
\vec r(t) = (t, t^2)
$$

Differentiate:

$$
\vec v(t) = (1, 2t)
$$

---

## 2. Magnitude of velocity

$$
|\vec v(t)| = \sqrt{1 + 4t^2}
$$

---

## 3. Arc length

$$
s = \int_0^1 \sqrt{1 + 4t^2}\,dt
$$

---

## 4. Analytical solution

Substitute

$$
u = 2t, \quad dt = \frac{du}{2}
$$

Then

$$
s = \frac{1}{2} \int_0^2 \sqrt{1 + u^2}\,du
$$

Use formula

$$
\int \sqrt{1 + u^2}\,du =
\frac{1}{2}\left(u\sqrt{1+u^2} + \ln(u + \sqrt{1+u^2})\right)
$$

So

$$
s = \frac{1}{4}
\left[
u\sqrt{1+u^2} + \ln(u + \sqrt{1+u^2})
\right]_0^2
$$

Evaluate:

$$
s = \frac{1}{4}\left(2\sqrt{5} + \ln(2 + \sqrt{5})\right)
$$

Final form:

$$
s = \frac{\sqrt{5}}{2} + \frac{1}{4}\ln(2 + \sqrt{5})
$$

Approximation:

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
s = \frac{\sqrt{5}}{2} + \frac{1}{4}\ln(2 + \sqrt{5})
$$
