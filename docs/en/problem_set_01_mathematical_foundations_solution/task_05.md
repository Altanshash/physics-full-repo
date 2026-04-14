# Problem 5 – Trajectory curvature and normal acceleration

## Given

For the ellipse

$$
x(t) = a\cos t, \qquad y(t) = b\sin t
$$

we need to:

1. determine the velocity vector and the acceleration vector,
2. determine the unit tangent vector
   $$
   \hat T(t) = \frac{\vec v(t)}{|\vec v(t)|},
   $$
3. decompose the acceleration into tangential and normal components,
4. use
   $$
   a_n = \frac{v^2}{R}
   $$
   to determine the radius of curvature at $t=0$,
5. compare the result with the special case of a circle, where $a=b$.

We also answer the physical interpretation questions.

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

## 2. Speed and unit tangent vector

The speed is the magnitude of the velocity:

$$
|\vec v(t)| = \sqrt{(-a\sin t)^2 + (b\cos t)^2}
$$

$$
|\vec v(t)| = \sqrt{a^2\sin^2 t + b^2\cos^2 t}
$$

Therefore, the unit tangent vector is

$$
\hat T(t) = \frac{\vec v(t)}{|\vec v(t)|}
$$

$$
\hat T(t) =
\frac{(-a\sin t,\; b\cos t)}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

So,

$$
\hat T(t) =
\left(
\frac{-a\sin t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}},
\frac{b\cos t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
\right)
$$

---

## 3. Tangential and normal components of acceleration

We write

$$
\vec a(t) = \vec a_t(t) + \vec a_n(t)
$$

where:

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

differentiate it:

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

So,

$$
\frac{d}{dt}(a^2\sin^2 t + b^2\cos^2 t)
=
2(a^2-b^2)\sin t\cos t
$$

Hence,

$$
a_t(t)
=
\frac{(a^2-b^2)\sin t\cos t}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

Therefore, the tangential acceleration vector is

$$
\vec a_t(t) = a_t(t)\,\hat T(t)
$$

---

### 3.2 Normal acceleration

For a plane curve, the magnitude of the normal acceleration is

$$
a_n(t) = \frac{|\vec v(t) \times \vec a(t)|}{|\vec v(t)|}
$$

Treat the vectors as 3D vectors with third coordinate equal to zero:

$$
\vec v(t) = (-a\sin t,\; b\cos t,\; 0)
$$

$$
\vec a(t) = (-a\cos t,\; -b\sin t,\; 0)
$$

Now compute the cross product.

Its first component is

$$
(b\cos t)(0) - (0)(-b\sin t) = 0
$$

Its second component is

$$
(0)(-a\cos t) - (-a\sin t)(0) = 0
$$

Its third component is

$$
(-a\sin t)(-b\sin t) - (b\cos t)(-a\cos t)
$$

$$
= ab\sin^2 t + ab\cos^2 t
$$

$$
= ab(\sin^2 t + \cos^2 t) = ab
$$

So,

$$
\vec v(t) \times \vec a(t) = (0,\; 0,\; ab)
$$

and therefore

$$
|\vec v(t) \times \vec a(t)| = ab
$$

Thus,

$$
a_n(t) = \frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

So the magnitude of the normal acceleration is

$$
a_n(t) = \frac{ab}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

The normal component vector itself is

$$
\vec a_n(t) = \vec a(t) - \vec a_t(t)
$$

---

## 4. Radius of curvature at $t=0$

We use the relation

$$
a_n = \frac{v^2}{R}
$$

Therefore,

$$
R = \frac{v^2}{a_n}
$$

Now evaluate everything at $t=0$.

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

Using the formula for $a_n(t)$:

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

## 5. Special case: circle $a=b$

If

$$
a=b=R_0,
$$

then the ellipse becomes a circle:

$$
x(t) = R_0\cos t, \qquad y(t) = R_0\sin t
$$

The velocity becomes

$$
\vec v(t) = (-R_0\sin t,\; R_0\cos t)
$$

and its magnitude is

$$
|\vec v(t)| = R_0
$$

So the speed is constant, which means

$$
a_t(t) = 0
$$

For the normal acceleration,

$$
a_n(t) = \frac{R_0^2}{\sqrt{R_0^2\sin^2 t + R_0^2\cos^2 t}}
$$

$$
a_n(t) = \frac{R_0^2}{R_0} = R_0
$$

Thus, in circular motion:

$$
a_t = 0, \qquad a_n = R_0
$$

Also, the radius of curvature is constant and equal to the radius of the circle:

$$
R = R_0
$$

---

# Physical interpretation

## 1. Does greater curvature imply greater normal acceleration?

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

Therefore, for the same speed, greater curvature means greater normal acceleration.

So the answer is: **yes**, if the speed is fixed.

---

## 2. Where is the ellipse more curved: at the end of the major or minor semi-axis?

At

$$
t=0
$$

the point is

$$
(a,0)
$$

and we found

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

Now:

- at $t=\frac{\pi}{2}$, the speed is $a$,
- at $t=\frac{\pi}{2}$, the normal acceleration is $b$,

so

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

Therefore, the ellipse is more curved at the ends of the **major semi-axis**, that is, near

$$
(\pm a, 0)
$$

---

## 3. Why does normal acceleration change the direction of motion?

Tangential acceleration changes the magnitude of the velocity, so it changes the speed.

Normal acceleration is perpendicular to the velocity vector, so it changes the direction of the velocity instead of its magnitude.

Therefore, normal acceleration is responsible for turning the motion and bending the trajectory.

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
a_t = 0, \qquad a_n = R_0, \qquad R = R_0
$$

## Physical meaning

- Greater curvature gives greater normal acceleration if the speed is fixed.
- The ellipse is more curved at the ends of the major semi-axis.
- Tangential acceleration changes speed, while normal acceleration changes direction.
