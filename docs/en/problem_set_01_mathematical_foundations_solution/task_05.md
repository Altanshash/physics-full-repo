# Problem 5 – Trajectory curvature and normal acceleration

## Given

For an ellipse,

$$
x = a\cos t, \qquad y = b\sin t
$$

1. Determine the velocity vector $\vec v(t)$ and the acceleration vector $\vec a(t)$.

2. Determine the unit tangent vector to the trajectory.

$$
\hat T(t) = \frac{\vec v(t)}{|\vec v(t)|}
$$

3. Decompose the acceleration into tangential and normal components.

$$
\vec a(t) = \vec a_t(t) + \vec a_n(t)
$$

Determine the magnitude of the normal acceleration.

$$
a_n(t) = |\vec a_n(t)|
$$

4. Using the relation

$$
a_n = \frac{v^2}{R}
$$

determine the radius of curvature of the trajectory at the point $t=0$.

5. Compare the result with the case of a circle $a=b$.

---

## 1. Velocity vector and acceleration vector

The position vector is

$$
\vec r(t) = (a\cos t,\; b\sin t)
$$

Differentiate each component.

### Velocity vector

$$
\vec v(t) = \frac{d\vec r}{dt} = (-a\sin t,\; b\cos t)
$$

### Acceleration vector

$$
\vec a(t) = \frac{d\vec v}{dt} = (-a\cos t,\; -b\sin t)
$$

---

## 2. Unit tangent vector

First compute the speed:

$$
|\vec v(t)| = \sqrt{(-a\sin t)^2 + (b\cos t)^2}
$$

$$
|\vec v(t)| = \sqrt{a^2\sin^2 t + b^2\cos^2 t}
$$

Now use the definition

$$
\hat T(t) = \frac{\vec v(t)}{|\vec v(t)|}
$$

Therefore,

$$
\hat T(t) =
\frac{(-a\sin t,\; b\cos t)}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

---

## 3. Tangential and normal components of acceleration

We write

$$
\vec a(t) = \vec a_t(t) + \vec a_n(t)
$$

where $\vec a_t(t)$ is tangential and $\vec a_n(t)$ is normal.

### 3.1 Tangential acceleration

The tangential acceleration magnitude is

$$
a_t(t) = \frac{\vec v(t)\cdot\vec a(t)}{|\vec v(t)|}
$$

First compute the dot product:

$$
\vec v(t)\cdot\vec a(t)
=
(-a\sin t)(-a\cos t) + (b\cos t)(-b\sin t)
$$

$$
\vec v(t)\cdot\vec a(t)
=
a^2\sin t\cos t - b^2\sin t\cos t
$$

$$
\vec v(t)\cdot\vec a(t)
=
(a^2-b^2)\sin t\cos t
$$

Since

$$
|\vec v(t)| = \sqrt{a^2\sin^2 t + b^2\cos^2 t},
$$

we obtain

$$
a_t(t) =
\frac{(a^2-b^2)\sin t\cos t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

Hence,

$$
\vec a_t(t) = a_t(t)\,\hat T(t)
$$

### 3.2 Normal acceleration

The magnitude of the normal acceleration is

$$
a_n(t) = \frac{|\vec v(t)\times\vec a(t)|}{|\vec v(t)|}
$$

Treat the vectors as 3D vectors:

$$
\vec v(t) = (-a\sin t,\; b\cos t,\; 0)
$$

$$
\vec a(t) = (-a\cos t,\; -b\sin t,\; 0)
$$

Then

$$
\vec v(t)\times\vec a(t) = (0,\;0,\;ab)
$$

so

$$
|\vec v(t)\times\vec a(t)| = ab
$$

Therefore,

$$
a_n(t) = \frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

Thus,

$$
a_n(t) = |\vec a_n(t)| = \frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

and

$$
\vec a_n(t) = \vec a(t) - \vec a_t(t)
$$

---

## 4. Radius of curvature at the point $t=0$

Use

$$
a_n = \frac{v^2}{R}
$$

so

$$
R = \frac{v^2}{a_n}
$$

At $t=0$:

$$
\vec v(0) = (-a\sin 0,\; b\cos 0) = (0,\; b)
$$

Hence,

$$
|\vec v(0)| = b
$$

so

$$
v(0)^2 = b^2
$$

Also,

$$
a_n(0) = \frac{ab}{\sqrt{a^2\sin^2 0 + b^2\cos^2 0}}
$$

$$
a_n(0) = \frac{ab}{b} = a
$$

Therefore,

$$
R(0) = \frac{b^2}{a}
$$

---

## 5. Comparison with the case of a circle $a=b$

If

$$
a=b=r,
$$

then

$$
x = r\cos t, \qquad y = r\sin t
$$

The speed is

$$
|\vec v(t)| = r
$$

so it is constant. Therefore,

$$
a_t(t) = 0
$$

Also,

$$
a_n(t) = \frac{r^2}{r} = r
$$

Thus, for a circle,

$$
a_t = 0, \qquad a_n = r, \qquad R = r
$$

---

## Physical interpretation

### 1. Does a greater trajectory curvature imply a greater normal acceleration?

Since

$$
a_n = \frac{v^2}{R}
$$

and

$$
\kappa = \frac{1}{R},
$$

we get

$$
a_n = v^2\kappa
$$

So for fixed speed, greater curvature implies greater normal acceleration.

### 2. Where on the ellipse is the trajectory more curved: at the end of the major or minor semi-axis?

At $t=0$:

$$
R(0) = \frac{b^2}{a}
$$

At $t=\frac{\pi}{2}$:

$$
R\left(\frac{\pi}{2}\right) = \frac{a^2}{b}
$$

The curve is more curved where the radius is smaller. If $a>b$, then

$$
\frac{b^2}{a} < \frac{a^2}{b}
$$

So the ellipse is more curved at the ends of the major semi-axis, near $(\pm a,0)$.

### 3. Why can normal acceleration be interpreted as the cause of the change in the direction of motion?

Tangential acceleration changes the speed.  
Normal acceleration is perpendicular to the velocity, so it changes the direction of motion.

---

## Final answers

$$
\vec v(t) = (-a\sin t,\; b\cos t)
$$

$$
\vec a(t) = (-a\cos t,\; -b\sin t)
$$

$$
\hat T(t) =
\frac{(-a\sin t,\; b\cos t)}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

$$
a_t(t) =
\frac{(a^2-b^2)\sin t\cos t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

$$
a_n(t) =
\frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

$$
R(0) = \frac{b^2}{a}
$$

For $a=b=r$:

$$
a_t = 0, \qquad a_n = r, \qquad R = r
$$
