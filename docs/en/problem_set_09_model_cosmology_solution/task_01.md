# Problem Set 9 – Model Cosmology: From Epicycles to Gravity

## Problem 1 – Ptolemy's Model

## Given

A planet moves as the sum of two circular motions:

- motion along the deferent;
- motion along the epicycle.

The parametric equations are:

$$
x(t) = R\cos(\omega t) + r\cos(\Omega t)
$$

$$
y(t) = R\sin(\omega t) + r\sin(\Omega t)
$$

where:

$$
R
$$

is the radius of the deferent,

$$
r
$$

is the radius of the epicycle,

$$
\omega
$$

is the angular velocity of the deferent,

$$
\Omega
$$

is the angular velocity of the epicycle,

$$
t
$$

is time.

---

## Solution

### 1. Motion Along the Deferent

The coordinates of motion along the main circle are:

$$
x_R(t) = R\cos(\omega t)
$$

$$
y_R(t) = R\sin(\omega t)
$$

---

### 2. Motion Along the Epicycle

The coordinates of motion along the epicycle are:

$$
x_r(t) = r\cos(\Omega t)
$$

$$
y_r(t) = r\sin(\Omega t)
$$

---

### 3. Total Parametric Equations

The total position is the sum of both motions:

$$
x(t) = x_R(t) + x_r(t)
$$

$$
y(t) = y_R(t) + y_r(t)
$$

Therefore:

$$
x(t) = R\cos(\omega t) + r\cos(\Omega t)
$$

$$
y(t) = R\sin(\omega t) + r\sin(\Omega t)
$$

---

### 4. Ecliptic Longitude

The apparent angular position is:

$$
\varphi(t) = \arctan\left(\frac{y(t)}{x(t)}\right)
$$

In the HTML program, the angle should be calculated using:

```js
phi = Math.atan2(y, x);
