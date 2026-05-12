# Problem Set 9 – Model Cosmology: From Epicycles to Gravity

## Problem 1 – Ptolemy's Model

## Given

A planet moves as the sum of two circular motions:

1. Motion along the deferent, which is the main circle.
2. Motion along the epicycle, which is the smaller circle.

The parametric representation is:

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

### 1. Parametric Equations of the Trajectory

The position vector of the planet is the sum of two circular motions:

$$\vec{r}(t) = \vec{r}_R(t) + \vec{r}_r(t)$$

For the deferent:

$$\vec{r}_R(t) = (R\cos(\omega t),\ R\sin(\omega t))$$

For the epicycle:

$$\vec{r}_r(t) = (r\cos(\Omega t),\ r\sin(\Omega t))$$

Therefore:

$$x(t) = R\cos(\omega t) + r\cos(\Omega t)$$

$$y(t) = R\sin(\omega t) + r\sin(\Omega t)$$

---

### 2. Angular Projection

The apparent angular position of the planet is:

$$\varphi(t) = \arctan\left(\frac{y(t)}{x(t)}\right)$$

More correctly, to determine the quadrant:

$$\varphi(t) = \operatorname{atan2}(y(t), x(t))$$

---

### 3. Condition for Retrograde Motion

Retrograde motion occurs when the angular position decreases with time.

Therefore, the condition is:

$$\frac{d\varphi}{dt} < 0$$

The angular velocity of the projection is:

$$\frac{d\varphi}{dt} = \frac{x(t)y'(t) - y(t)x'(t)}{x^2(t) + y^2(t)}$$

where:

$$x'(t) = -R\omega \sin(\omega t) - r\Omega \sin(\Omega t)$$

$$y'(t) = R\omega \cos(\omega t) + r\Omega \cos(\Omega t)$$

Since the denominator is always positive, retrograde motion occurs when:

$$x(t)y'(t) - y(t)x'(t) < 0$$

---

### 4. Moments of Direction Change

The direction of angular motion changes when:

$$\frac{d\varphi}{dt} = 0$$

So the moments of change are determined by:

$$x(t)y'(t) - y(t)x'(t) = 0$$

These are the points where the angular projection changes from direct motion to retrograde motion or from retrograde motion to direct motion.

---

## HTML Application Requirements

The HTML application should include:

1. Sliders for:

$$R,\ r,\ \omega,\ \Omega$$

2. A trajectory trace of the planet.

3. A graph of ecliptic longitude:

$$\varphi(t)$$

4. A visual indication of retrograde motion when:

$$\frac{d\varphi}{dt} < 0$$

---

## Conclusion

Ptolemy's model represents planetary motion as a combination of a deferent and an epicycle.

The trajectory is described by:

$$x(t) = R\cos(\omega t) + r\cos(\Omega t)$$

$$y(t) = R\sin(\omega t) + r\sin(\Omega t)$$

Retrograde motion appears when the apparent angular velocity becomes negative:

$$\frac{d\varphi}{dt} < 0$$

The moments when the planet changes direction are found from:

$$x(t)y'(t) - y(t)x'(t) = 0$$

This model explains how loop-like apparent motion can arise from the combination of circular motions.
