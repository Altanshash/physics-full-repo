## Problem 2 – Parametric trajectory, velocity, and acceleration

### Given

The trajectory is given by

r(t) = (t^2, sin t, 5)

We need to determine:

- the velocity vector v(t),
- the acceleration vector a(t),
- the value of |v(1)|,
- the dot product v · a,
- the cross product v × a.

---

## 1. Velocity vector

The velocity is the derivative of the position vector:

v(t) = dr/dt

Since

r(t) = (t^2, sin t, 5),

differentiate each component:

- d/dt (t^2) = 2t
- d/dt (sin t) = cos t
- d/dt (5) = 0

Therefore,

v(t) = (2t, cos t, 0)

---

## 2. Acceleration vector

The acceleration is the derivative of the velocity vector:

a(t) = dv/dt

Using

v(t) = (2t, cos t, 0),

differentiate again:

- d/dt (2t) = 2
- d/dt (cos t) = -sin t
- d/dt (0) = 0

So,

a(t) = (2, -sin t, 0)

---

## 3. Magnitude of the velocity at t = 1

First compute the velocity at t = 1:

v(1) = (2, cos 1, 0)

The magnitude of a vector (x, y, z) is

|v| = sqrt(x^2 + y^2 + z^2)

Hence,

|v(1)| = sqrt(2^2 + (cos 1)^2 + 0^2)

|v(1)| = sqrt(4 + cos^2 1)

Using cos 1 ≈ 0.5403:

|v(1)| ≈ sqrt(4.2919) ≈ 2.07

So,

|v(1)| ≈ 2.07

---

## 4. Dot product v · a

We have

v(t) = (2t, cos t, 0)

a(t) = (2, -sin t, 0)

The dot product is

v · a = (2t)(2) + (cos t)(-sin t) + 0·0

So,

v · a = 4t - sin t cos t

---

## 5. Cross product v × a

For two vectors

(u1, u2, u3) × (w1, w2, w3)
= (u2w3 - u3w2, u3w1 - u1w3, u1w2 - u2w1)

Here,

v(t) = (2t, cos t, 0)

a(t) = (2, -sin t, 0)

Now compute each component.

First component:

v2 a3 - v3 a2
= (cos t)(0) - (0)(-sin t)
= 0

Second component:

v3 a1 - v1 a3
= (0)(2) - (2t)(0)
= 0

Third component:

v1 a2 - v2 a1
= (2t)(-sin t) - (cos t)(2)
= -2t sin t - 2 cos t

Therefore,

v × a = (0, 0, -2t sin t - 2 cos t)

---

## Final answers

- v(t) = (2t, cos t, 0)
- a(t) = (2, -sin t, 0)
- |v(1)| = sqrt(4 + cos^2 1) ≈ 2.07
- v · a = 4t - sin t cos t
- v × a = (0, 0, -2t sin t - 2 cos t)
