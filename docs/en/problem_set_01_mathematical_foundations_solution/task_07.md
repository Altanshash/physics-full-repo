# Problem 7 – Work of a force along a trajectory

## Given

The force field is

$$
\vec F(x,y) = (y, 2x)
$$

The trajectory is

$$
x=t, \qquad y=t^2, \qquad t\in[0,1]
$$

Determine:

1. the velocity vector $\vec v(t)$,
2. the work done by the force along the trajectory,
3. the line integral as a Riemann sum.

---

## 1. Velocity vector

The position vector is

$$
\vec r(t) = (t, t^2)
$$

Differentiate:

$$
\vec v(t) = \vec r\,'(t) = (1, 2t)
$$

---

## 2. Work done by the force

The work is

$$
W = \int_C \vec F \cdot d\vec r
$$

Using the parameterization $\vec r(t) = (t,t^2)$, we write

$$
W = \int_0^1 \vec F(\vec r(t)) \cdot \vec r\,'(t)\,dt
$$

First compute the force along the curve:

$$
\vec F(\vec r(t)) = \vec F(t,t^2) = (t^2, 2t)
$$

Now compute the dot product:

$$
\vec F(\vec r(t)) \cdot \vec r\,'(t)
= (t^2,2t)\cdot(1,2t)
$$

$$
\vec F(\vec r(t)) \cdot \vec r\,'(t)
= t^2 + 4t^2 = 5t^2
$$

Therefore,

$$
W = \int_0^1 5t^2\,dt
$$

$$
W = 5\left[\frac{t^3}{3}\right]_0^1
$$

$$
W = \frac{5}{3}
$$

---

## 3. Riemann sum form

Write the integral

$$
W = \int_0^1 5t^2\,dt
$$

as a Riemann sum.

Divide the interval $[0,1]$ into $N$ equal parts:

$$
\Delta t = \frac{1}{N}, \qquad t_i = \frac{i}{N}
$$

Then

$$
W = \lim_{N\to\infty} \sum_{i=1}^N 5t_i^2\,\Delta t
$$

Substitute $t_i=\frac{i}{N}$ and $\Delta t=\frac{1}{N}$:

$$
W = \lim_{N\to\infty} \sum_{i=1}^N 5\left(\frac{i}{N}\right)^2 \frac{1}{N}
$$

$$
W = \lim_{N\to\infty} \frac{5}{N^3}\sum_{i=1}^N i^2
$$

Using

$$
\sum_{i=1}^N i^2 = \frac{N(N+1)(2N+1)}{6}
$$

we get

$$
W = \lim_{N\to\infty} \frac{5}{N^3}\cdot\frac{N(N+1)(2N+1)}{6}
$$

$$
W = \lim_{N\to\infty} \frac{5(N+1)(2N+1)}{6N^2}
$$

As $N\to\infty$,

$$
W = \frac{5}{3}
$$

So the numerical Riemann sum converges to the same value.

---

## Final answers

$$
\vec v(t) = (1,2t)
$$

$$
W = \frac{5}{3}
$$

$$
W = \lim_{N\to\infty} \sum_{i=1}^N 5\left(\frac{i}{N}\right)^2 \frac{1}{N}
$$
