# Problem 4 – Kepler's First and Second Laws

## Given

Kepler's first law states that planets move in elliptical orbits, with the Sun located at one focus of the ellipse.

The elliptical orbit in polar form is:

$$
r(\theta)=\frac{a(1-e^2)}{1+e\cos\theta}
$$

Where:

- $r(\theta)$ is the distance from the Sun to the planet.
- $a$ is the semi-major axis.
- $e$ is the eccentricity.
- $\theta$ is the polar angle.

The swept area is calculated by:

$$
A=\frac{1}{2}\int r^2 d\theta
$$

---

## Solution

### 1. Elliptical Orbit

The orbit is given by:

$$
r(\theta)=\frac{a(1-e^2)}{1+e\cos\theta}
$$

To draw the orbit, we convert polar coordinates to Cartesian coordinates:

$$
x(\theta)=r(\theta)\cos\theta
$$

$$
y(\theta)=r(\theta)\sin\theta
$$

Substituting $r(\theta)$:

$$
x(\theta)=
\frac{a(1-e^2)\cos\theta}
{1+e\cos\theta}
$$

$$
y(\theta)=
\frac{a(1-e^2)\sin\theta}
{1+e\cos\theta}
$$

This gives an ellipse with the Sun at one focus.

---

### 2. Effect of Eccentricity

The eccentricity $e$ controls the shape of the orbit.

If:

$$
e=0
$$

the orbit is a circle.

If:

$$
0<e<1
$$

the orbit is an ellipse.

As $e$ increases, the ellipse becomes more stretched.

---

### 3. Area Swept in Equal Time Intervals

Kepler's second law states that a line connecting the Sun and a planet sweeps out equal areas in equal times.

The swept area is:

$$
A=\frac{1}{2}\int_{\theta_1}^{\theta_2} r^2 d\theta
$$

For numerical calculation, the integral can be approximated by a sum:

$$
A\approx
\frac{1}{2}
\sum r_i^2\Delta\theta_i
$$

where:

$$
\Delta\theta_i=\theta_{i+1}-\theta_i
$$

This allows us to compare swept areas over equal time intervals.

---

### 4. Verification of the Law of Equal Areas

If the time intervals are equal, the swept areas should be approximately equal.

In the animation:

- The planet moves faster near the Sun.
- The planet moves slower when it is far from the Sun.
- The swept sectors have nearly equal areas for equal time intervals.

This confirms Kepler's second law.

---

## HTML Requirements

The HTML visualization should include:

- Visualization of the focus
- Drawing of area sectors
- Dynamic area comparison
- Slider for eccentricity $e$

---

## Conclusion

Kepler's first law states that planetary orbits are ellipses with the Sun at one focus.

The orbit is described by:

$$
r(\theta)=\frac{a(1-e^2)}{1+e\cos\theta}
$$

Changing the eccentricity $e$ changes the shape of the orbit. When $e=0$, the orbit is circular. As $e$ increases, the orbit becomes more elongated.

Kepler's second law states that equal time intervals sweep out equal areas:

$$
A=\frac{1}{2}\int r^2 d\theta
$$

The numerical area calculation confirms that the swept areas are approximately equal, even though the planet moves faster near the Sun and slower farther away.
