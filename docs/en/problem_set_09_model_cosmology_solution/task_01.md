# Problem Set 9 – Model Cosmology: From Epicycles to Gravity

## Problem 1 – Ptolemy's Model

## Given

A planet moves as the sum of two circular motions:

- motion along the deferent, which is the main circle;
- motion along the epicycle, which is the smaller circle.

The parametric equations are:

$$x(t) = R\cos(\omega t) + r\cos(\Omega t)$$

$$y(t) = R\sin(\omega t) + r\sin(\Omega t)$$

where:

$$R$$

is the radius of the deferent,

$$r$$

is the radius of the epicycle,

$$\omega$$

is the angular velocity of the deferent,

$$\Omega$$

is the angular velocity of the epicycle,

$$t$$

is time.

---

## Solution

### 1. Parametric Equations of Motion

The planet's position is the sum of two circular motions.

For the deferent:

$$x_R(t) = R\cos(\omega t)$$

$$y_R(t) = R\sin(\omega t)$$

For the epicycle:

$$x_r(t) = r\cos(\Omega t)$$

$$y_r(t) = r\sin(\Omega t)$$

Therefore, the total motion is:

$$x(t) = x_R(t) + x_r(t)$$

$$y(t) = y_R(t) + y_r(t)$$

So:

$$x(t) = R\cos(\omega t) + r\cos(\Omega t)$$

$$y(t) = R\sin(\omega t) + r\sin(\Omega t)$$

---

### 2. Ecliptic Longitude

The apparent angular position is:

$$\varphi(t) = \arctan\left(\frac{y(t)}{x(t)}\right)$$

In the HTML code, it is better to use the JavaScript function:

```js
Math.atan2(y, x)
