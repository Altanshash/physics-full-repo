# Problem Set 9 – Model Cosmology: From Epicycles to Gravity

# Problem 1 – Ptolemy’s Model

## Given

The motion of a planet is represented as the sum of two circular motions:

1. Motion along the deferent, which is the main circle.
2. Motion along the epicycle.

The parametric equations are:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x(t)=R\cos(\omega%20t)+r\cos(\Omega%20t)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y(t)=R\sin(\omega%20t)+r\sin(\Omega%20t)" />
</p>

Where:

- **R** is the radius of the deferent.
- **r** is the radius of the epicycle.
- **ω** is the angular velocity of the deferent.
- **Ω** is the angular velocity of the epicycle.
- **t** is time.

---

# Solution

## 1. Parametric Equations of the Trajectory

The position of the planet is the sum of the deferent motion and the epicycle motion.

For the deferent:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x_1(t)=R\cos(\omega%20t)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y_1(t)=R\sin(\omega%20t)" />
</p>

For the epicycle:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x_2(t)=r\cos(\Omega%20t)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y_2(t)=r\sin(\Omega%20t)" />
</p>

Adding these two motions:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x(t)=x_1(t)+x_2(t)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y(t)=y_1(t)+y_2(t)" />
</p>

Therefore:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x(t)=R\cos(\omega%20t)+r\cos(\Omega%20t)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y(t)=R\sin(\omega%20t)+r\sin(\Omega%20t)" />
</p>

These equations describe the trajectory of the planet.

---

## 2. Ecliptic Longitude

The ecliptic longitude is the angular position of the planet as seen from the origin.

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\varphi(t)=\arctan\left(\frac{y(t)}{x(t)}\right)" />
</p>

Substituting the parametric equations:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\varphi(t)=\arctan\left(\frac{R\sin(\omega%20t)+r\sin(\Omega%20t)}{R\cos(\omega%20t)+r\cos(\Omega%20t)}\right)" />
</p>

---

## 3. Condition for Retrograde Motion

Retrograde motion occurs when the apparent angular motion becomes negative.

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\frac{d\varphi}{dt}<0" />
</p>

For a parametric curve, the angular velocity is:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\frac{d\varphi}{dt}=\frac{x(t)y'(t)-y(t)x'(t)}{x^2(t)+y^2(t)}" />
</p>

The derivatives are:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x'(t)=-R\omega\sin(\omega%20t)-r\Omega\sin(\Omega%20t)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y'(t)=R\omega\cos(\omega%20t)+r\Omega\cos(\Omega%20t)" />
</p>

Since the denominator is positive, retrograde motion occurs when:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x(t)y'(t)-y(t)x'(t)<0" />
</p>

After simplification:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?R^2\omega+r^2\Omega+Rr(\omega+\Omega)\cos((\omega-\Omega)t)<0" />
</p>

Thus, this is the condition for retrograde motion.

---

## 4. Moments of Change in Direction

The direction changes when the angular velocity becomes zero.

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\frac{d\varphi}{dt}=0" />
</p>

Therefore:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?R^2\omega+r^2\Omega+Rr(\omega+\Omega)\cos((\omega-\Omega)t)=0" />
</p>

Solving for the cosine term:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\cos((\omega-\Omega)t)=-\frac{R^2\omega+r^2\Omega}{Rr(\omega+\Omega)}" />
</p>

The moments of direction change are:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?t_n=\frac{\pm\arccos\left(-\frac{R^2\omega+r^2\Omega}{Rr(\omega+\Omega)}\right)+2\pi n}{\omega-\Omega}" />
</p>

where **n** is an integer.

The solution exists only if:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\left|\frac{R^2\omega+r^2\Omega}{Rr(\omega+\Omega)}\right|\leq1" />
</p>

---

# HTML Requirements

The HTML model must include:

- Sliders for **R**, **r**, **ω**, and **Ω**
- A trajectory trace of the planet
- A graph of the ecliptic longitude **φ(t)**

The ecliptic longitude is:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\varphi(t)=\arctan\left(\frac{R\sin(\omega%20t)+r\sin(\Omega%20t)}{R\cos(\omega%20t)+r\cos(\Omega%20t)}\right)" />
</p>

---

# Conclusion

Ptolemy’s model describes planetary motion as a combination of two circular motions: motion along the deferent and motion along the epicycle.

The trajectory is described by:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x(t)=R\cos(\omega%20t)+r\cos(\Omega%20t)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y(t)=R\sin(\omega%20t)+r\sin(\Omega%20t)" />
</p>

Retrograde motion occurs when:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\frac{d\varphi}{dt}<0" />
</p>

The moments when the planet changes its apparent direction are found from:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\frac{d\varphi}{dt}=0" />
</p>

Thus, retrograde motion depends on **R**, **r**, **ω**, and **Ω**.
