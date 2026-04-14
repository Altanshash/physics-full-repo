# Problem 5 – Trajectory curvature and normal acceleration

## Given

For the ellipse

$$
x(t) = a\cos t, \qquad y(t) = b\sin t
$$

we need to:

1. determine the velocity vector $\vec v(t)$ and the acceleration vector $\vec a(t)$,
2. determine the unit tangent vector
   $$
   \hat T(t) = \frac{\vec v(t)}{|\vec v(t)|},
   $$
3. decompose the acceleration into tangential and normal components
   $$
   \vec a(t) = \vec a_t(t) + \vec a_n(t),
   $$
   and determine the magnitude of the normal acceleration
   $$
   a_n(t) = |\vec a_n(t)|,
   $$
4. using
   $$
   a_n = \frac{v^2}{R},
   $$
   determine the radius of curvature at $t=0$,
5. compare the result with the special case of a circle $a=b$.

We also answer the physical interpretation questions.

---

## 1. Velocity and acceleration

The position vector is

$$
\vec r(t) = (a\cos t, b\sin t)
$$

Differentiate componentwise.

### Velocity

$$
\vec v(t) = \frac{d\vec r}{dt} = (-a\sin t, b\cos t)
$$

### Acceleration

$$
\vec a(t) = \frac{d\vec v}{dt} = (-a\cos t, -b\sin t)
$$

The speed is

$$
|\vec v(t)| = \sqrt{(-a\sin t)^2 + (b\cos t)^2}
$$

$$
|\vec v(t)| = \sqrt{a^2\sin^2 t + b^2\cos^2 t}
$$

---

## 2. Unit tangent vector

By definition,

$$
\hat T(t) = \frac{\vec v(t)}{|\vec v(t)|}
$$

Therefore,

$$
\hat T(t) =
\frac{(-a\sin t, b\cos t)}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

So the unit tangent vector is

$$
\hat T(t) =
\left(
\frac{-a\sin t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}},
\frac{b\cos t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
\right)
$$

---

## 3. Tangential and normal components of acceleration

We use the standard decomposition

$$
\vec a = \vec a_t + \vec a_n
$$

where the tangential component is parallel to $\vec v$ and the normal component is perpendicular to $\vec v$.

### 3.1 Tangential acceleration magnitude

The tangential acceleration magnitude is

$$
a_t = \frac{d}{dt} |\vec v|
$$

Since

$$
|\vec v| = \sqrt{a^2\sin^2 t + b^2\cos^2 t},
$$

differentiate:

$$
a_t
=
\frac{1}{2\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
\cdot
\frac{d}{dt}(a^2\sin^2 t + b^2\cos^2 t)
$$

Now,

$$
\frac{d}{dt}(a^2\sin^2 t + b^2\cos^2 t)
=
2a^2\sin t\cos t - 2b^2\sin t\cos t
$$

$$
=
2(a^2-b^2)\sin t\cos t
$$

Therefore,

$$
a_t
=
\frac{(a^2-b^2)\sin t\cos t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

Thus the tangential acceleration vector is

$$
\vec a_t = a_t \hat T
$$

so

$$
\vec a_t
=
\frac{(a^2-b^2)\sin t\cos t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
\hat T(t)
$$

---

### 3.2 Normal acceleration magnitude

A convenient formula is

$$
a_n = \sqrt{|\vec a|^2 - a_t^2}
$$

but for plane curves it is simpler to use

$$
a_n = \frac{|\vec v \times \vec a|}{|\vec v|}
$$

Treat the 2D vectors as 3D vectors with third coordinate zero:

$$
\vec v = (-a\sin t, b\cos t, 0), \qquad
\vec a = (-a\cos t, -b\sin t, 0)
$$

Then

$$
\vec v \times \vec a
=
(0,0,(-a\sin t)(-b\sin t) - (b\cos t)(-a\cos t))
$$

$$
=
(0,0,ab\sin^2 t + ab\cos^2 t)
$$

$$
=
(0,0,ab)
$$

Hence

$$
|\vec v \times \vec a| = ab
$$

Therefore,

$$
a_n(t) = \frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

So the magnitude of the normal acceleration is

$$
a_n(t) = \frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

The normal acceleration vector is

$$
\vec a_n = \vec a - \vec a_t
$$

---

## 4. Radius of curvature at $t=0$

We use

$$
a_n = \frac{v^2}{R}
$$

So

$$
R = \frac{v^2}{a_n}
$$

At $t=0$:

### Step 1. Velocity at $t=0$

$$
\vec v(0) = (-a\sin 0, b\cos 0) = (0,b)
$$

Thus

$$
|\vec v(0)| = b
$$

### Step 2. Normal acceleration at $t=0$

From the formula above,

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

So the radius of curvature at $t=0$ is

$$
R(0) = \frac{b^2}{a}
$$

---

## 5. Special case: circle $a=b$

If $a=b=R_0$, then the ellipse becomes a circle:

$$
x(t) = R_0\cos t, \qquad y(t) = R_0\sin t
$$

Then

$$
|\vec v| = R_0
$$

is constant, so the tangential acceleration is zero:

$$
a_t = 0
$$

Also,

$$
a_n = \frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
\quad \Longrightarrow \quad
a_n = \frac{R_0^2}{R_0} = R_0
$$

Thus for a circle the acceleration is purely normal, and the radius of curvature is constant:

$$
R = R_0
$$

This matches the usual result for circular motion.

---

# Physical interpretation

## 1. Does greater curvature imply greater normal acceleration?

From the relation

$$
a_n = \frac{v^2}{R}
$$

and curvature

$$
\kappa = \frac{1}{R},
$$

we get

$$
a_n = v^2 \kappa
$$

So for the same speed, greater curvature means greater normal acceleration.

Therefore, **yes**: greater curvature implies greater normal acceleration if the speed is fixed.

---

## 2. Where is the ellipse more curved: at the end of the major or minor semi-axis?

At the point $t=0$, the point on the ellipse is

$$
(a,0)
$$

and we found

$$
R(0) = \frac{b^2}{a}
$$

If we evaluate similarly at the top point $t=\frac{\pi}{2}$, we get

$$
R\left(\frac{\pi}{2}\right) = \frac{a^2}{b}
$$

Curvature is larger where the radius of curvature is smaller.

So:

- at $(a,0)$, the radius is $\frac{b^2}{a}$,
- at $(0,b)$, the radius is $\frac{a^2}{b}$.

If $a>b$, then

$$
\frac{b^2}{a} < \frac{a^2}{b}
$$

so the ellipse is more curved at the ends of the **major semi-axis**, that is, near $(\pm a,0)$.

---

## 3. Why can normal acceleration be interpreted as the cause of the change in direction of motion?

Tangential acceleration changes the magnitude of the velocity, that is, the speed.

Normal acceleration is perpendicular to the velocity vector, so it does not change the speed directly. Instead, it changes the direction of the velocity vector.

Therefore, normal acceleration is responsible for bending the trajectory and changing the direction of motion.

---

# Final answers

## Velocity and acceleration

$$
\vec v(t) = (-a\sin t, b\cos t)
$$

$$
\vec a(t) = (-a\cos t, -b\sin t)
$$

## Unit tangent vector

$$
\hat T(t) =
\frac{(-a\sin t, b\cos t)}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

## Tangential acceleration magnitude

$$
a_t =
\frac{(a^2-b^2)\sin t\cos t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

## Normal acceleration magnitude

$$
a_n =
\frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

## Radius of curvature at $t=0$

$$
R(0) = \frac{b^2}{a}
$$

## Circle case $a=b=R_0$

$$
a_t = 0, \qquad a_n = R_0, \qquad R = R_0
$$

## Physical interpretation

- Greater curvature means greater normal acceleration when speed is fixed.
- The ellipse is more curved at the ends of the major semi-axis.
- Normal acceleration changes the direction of motion, while tangential acceleration changes the speed.
