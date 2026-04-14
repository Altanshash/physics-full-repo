# Problem 5 – Trajectory curvature and normal acceleration

## Given

For the ellipse

$$
x(t) = a\cos t, \qquad y(t) = b\sin t
$$

determine:

1. the velocity vector $\vec v(t)$ and the acceleration vector $\vec a(t)$,
2. the unit tangent vector
   $$
   \hat T(t) = \frac{\vec v(t)}{|\vec v(t)|},
   $$
3. the decomposition of acceleration into tangential and normal components
   $$
   \vec a(t) = \vec a_t(t) + \vec a_n(t),
   $$
   and the magnitude of the normal acceleration
   $$
   a_n(t) = |\vec a_n(t)|,
   $$
4. using
   $$
   a_n = \frac{v^2}{R},
   $$
   determine the radius of curvature at the point $t=0$,
5. compare the result with the circle case $a=b$.

---

## 1. Velocity and acceleration

The position vector is

$$
\vec r(t) = (a\cos t,\; b\sin t)
$$

Differentiate componentwise.

### Velocity

$$
\vec v(t) = \frac{d\vec r}{dt} = (-a\sin t,\; b\cos t)
$$

### Acceleration

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

Therefore,

$$
\hat T(t) = \frac{\vec v(t)}{|\vec v(t)|}
$$

so

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

where

- $\vec a_t(t)$ is the tangential component,
- $\vec a_n(t)$ is the normal component.

### 3.1 Tangential acceleration

The tangential acceleration magnitude is

$$
a_t(t) = \frac{d}{dt}|\vec v(t)|
$$

Since

$$
|\vec v(t)| = \sqrt{a^2\sin^2 t + b^2\cos^2 t},
$$

differentiate:

$$
a_t(t)
=
\frac{1}{2\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
\cdot
\frac{d}{dt}(a^2\sin^2 t + b^2\cos^2 t)
$$

Now,

$$
\frac{d}{dt}(a^2\sin^2 t) = 2a^2\sin t\cos t
$$

and

$$
\frac{d}{dt}(b^2\cos^2 t) = -2b^2\sin t\cos t
$$

Hence,

$$
\frac{d}{dt}(a^2\sin^2 t + b^2\cos^2 t)
=
2(a^2-b^2)\sin t\cos t
$$

Therefore,

$$
a_t(t)
=
\frac{(a^2-b^2)\sin t\cos t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

So the tangential acceleration vector is

$$
\vec a_t(t) = a_t(t)\,\hat T(t)
$$

---

### 3.2 Normal acceleration

For plane motion,

$$
a_n(t) = \frac{|\vec v(t)\times\vec a(t)|}{|\vec v(t)|}
$$

Treat the vectors as 3D vectors with third coordinate zero:

$$
\vec v(t) = (-a\sin t,\; b\cos t,\; 0)
$$

$$
\vec a(t) = (-a\cos t,\; -b\sin t,\; 0)
$$

Now compute the cross product.

First component:

$$
(b\cos t)(0) - (0)(-b\sin t) = 0
$$

Second component:

$$
(0)(-a\cos t) - (-a\sin t)(0) = 0
$$

Third component:

$$
(-a\sin t)(-b\sin t) - (b\cos t)(-a\cos t)
$$

$$
= ab\sin^2 t + ab\cos^2 t
$$

$$
= ab(\sin^2 t + \cos^2 t) = ab
$$

Thus,

$$
\vec v(t)\times\vec a(t) = (0,\;0,\;ab)
$$

and therefore

$$
|\vec v(t)\times\vec a(t)| = ab
$$

Hence,

$$
a_n(t) = \frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

So the normal component magnitude is

$$
a_n(t) = \frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

Also,

$$
\vec a_n(t) = \vec a(t) - \vec a_t(t)
$$

---

## 4. Radius of curvature at $t=0$

We use

$$
a_n = \frac{v^2}{R}
$$

Therefore,

$$
R = \frac{v^2}{a_n}
$$

Now evaluate at $t=0$.

### Step 1. Velocity at $t=0$

$$
\vec v(0) = (-a\sin 0,\; b\cos 0) = (0,\; b)
$$

Hence,

$$
|\vec v(0)| = b
$$

So,

$$
v(0)^2 = b^2
$$

### Step 2. Normal acceleration at $t=0$

Using the formula above,

$$
a_n(0) = \frac{ab}{\sqrt{a^2\sin^2 0 + b^2\cos^2 0}}
$$

$$
a_n(0) = \frac{ab}{\sqrt{0 + b^2}} = \frac{ab}{b} = a
$$

### Step 3. Radius of curvature

Now substitute into

$$
R = \frac{v^2}{a_n}
$$

$$
R(0) = \frac{b^2}{a}
$$

Therefore, the radius of curvature at $t=0$ is

$$
R(0) = \frac{b^2}{a}
$$

---

## 5. Comparison with the circle case $a=b$

If

$$
a=b=r,
$$

then the ellipse becomes a circle:

$$
x(t) = r\cos t, \qquad y(t) = r\sin t
$$

In that case,

$$
|\vec v(t)| = \sqrt{r^2\sin^2 t + r^2\cos^2 t} = r
$$

So the speed is constant, and therefore

$$
a_t(t) = 0
$$

Also,

$$
a_n(t) = \frac{r^2}{\sqrt{r^2\sin^2 t + r^2\cos^2 t}} = \frac{r^2}{r} = r
$$

Thus for a circle,

$$
a_t = 0, \qquad a_n = r
$$

and the radius of curvature is constant:

$$
R = r
$$

---

# Physical interpretation

## 1. Does a greater trajectory curvature imply a greater normal acceleration?

We know that

$$
a_n = \frac{v^2}{R}
$$

and curvature is

$$
\kappa = \frac{1}{R}
$$

So,

$$
a_n = v^2\kappa
$$

Therefore, for fixed speed, greater curvature implies greater normal acceleration.

**Answer:** Yes, if the speed is fixed.

---

## 2. Where on the ellipse is the trajectory more curved: at the end of the major or minor semi-axis?

At

$$
t=0
$$

the point is

$$
(a,0)
$$

and the radius of curvature is

$$
R(0) = \frac{b^2}{a}
$$

At

$$
t=\frac{\pi}{2}
$$

the point is

$$
(0,b)
$$

Similarly,

$$
R\left(\frac{\pi}{2}\right) = \frac{a^2}{b}
$$

The curve is more curved where the radius of curvature is smaller.

If

$$
a>b,
$$

then

$$
\frac{b^2}{a} < \frac{a^2}{b}
$$

So the ellipse is more curved at the ends of the **major semi-axis**, that is, near

$$
(\pm a,0)
$$

---

## 3. Why can normal acceleration be interpreted as the cause of the change in the direction of motion?

Tangential acceleration changes the magnitude of the velocity, so it changes the speed.

Normal acceleration is perpendicular to the velocity vector, so it changes the direction of the velocity rather than its magnitude.

Therefore, normal acceleration is responsible for turning the motion and changing the direction of the trajectory.

---

# Final answers

## Velocity

$$
\vec v(t) = (-a\sin t,\; b\cos t)
$$

## Acceleration

$$
\vec a(t) = (-a\cos t,\; -b\sin t)
$$

## Unit tangent vector

$$
\hat T(t) =
\frac{(-a\sin t,\; b\cos t)}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

## Tangential acceleration magnitude

$$
a_t(t) =
\frac{(a^2-b^2)\sin t\cos t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

## Normal acceleration magnitude

$$
a_n(t) =
\frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

## Radius of curvature at $t=0$

$$
R(0) = \frac{b^2}{a}
$$

## Circle case

$$
a_t = 0, \qquad a_n = r, \qquad R = r
$$
