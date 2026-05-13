# Problem 2 – Copernicus's Model

## Given

Two planets move in circular orbits around the Sun.

The position of Earth is:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\vec{r}_Z(t)=R_Z(\cos(\omega_Zt),\sin(\omega_Zt))" />
</p>

The position of Mars is:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\vec{r}_M(t)=R_M(\cos(\omega_Mt),\sin(\omega_Mt))" />
</p>

Where:

- **RZ** is the orbital radius of Earth.
- **RM** is the orbital radius of Mars.
- **ωZ** is the angular velocity of Earth.
- **ωM** is the angular velocity of Mars.
- **t** is time.

The position of Mars relative to Earth is:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\vec{r}_{M/Z}(t)=\vec{r}_M(t)-\vec{r}_Z(t)" />
</p>

---

## Solution

## 1. Motion of Two Planets Around the Sun

In the heliocentric model, the Sun is placed at the center. Earth and Mars move around the Sun in circular orbits.

For Earth:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x_Z(t)=R_Z\cos(\omega_Zt)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y_Z(t)=R_Z\sin(\omega_Zt)" />
</p>

For Mars:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x_M(t)=R_M\cos(\omega_Mt)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y_M(t)=R_M\sin(\omega_Mt)" />
</p>

---

## 2. Position of Mars Relative to Earth

The relative position of Mars as seen from Earth is found by subtracting Earth's position from Mars's position.

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\vec{r}_{M/Z}(t)=\vec{r}_M(t)-\vec{r}_Z(t)" />
</p>

Therefore:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x_{M/Z}(t)=R_M\cos(\omega_Mt)-R_Z\cos(\omega_Zt)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y_{M/Z}(t)=R_M\sin(\omega_Mt)-R_Z\sin(\omega_Zt)" />
</p>

These equations describe the geocentric trajectory of Mars as observed from Earth.

---

## 3. Moments of Retrograde Motion

Retrograde motion occurs when the apparent angular velocity of Mars relative to Earth becomes negative.

The geocentric angle is:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\varphi(t)=\arctan\left(\frac{y_{M/Z}(t)}{x_{M/Z}(t)}\right)" />
</p>

Retrograde motion occurs when:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\frac{d\varphi}{dt}<0" />
</p>

For a parametric curve:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\frac{d\varphi}{dt}=\frac{x(t)y'(t)-y(t)x'(t)}{x^2(t)+y^2(t)}" />
</p>

Here:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x(t)=x_{M/Z}(t)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y(t)=y_{M/Z}(t)" />
</p>

The moments of retrogradation occur when:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\frac{d\varphi}{dt}=0" />
</p>

This means that the apparent motion changes direction. In the Copernican model, this happens because Earth, moving on an inner and faster orbit, overtakes Mars.

---

## 4. Comparison With the Epicycle Model

In Ptolemy's model, retrograde motion is explained using epicycles. The planet moves on a small circle whose center moves on a larger circle.

In Copernicus's model, retrograde motion appears naturally from the relative motion of Earth and Mars.

The geocentric trajectory in the Copernican model has a loop-like shape similar to the epicycle model, but it is caused by the observer's motion.

---

# HTML Requirements

The HTML simulation should include:

- A heliocentric view
- A geocentric view
- A reference frame switch

The heliocentric view shows Earth and Mars orbiting the Sun.

The geocentric view shows the apparent motion of Mars as seen from Earth.

---

# Conclusion

Copernicus's model explains retrograde motion using the motion of planets around the Sun.

Earth and Mars move in circular orbits:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\vec{r}_Z(t)=R_Z(\cos(\omega_Zt),\sin(\omega_Zt))" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\vec{r}_M(t)=R_M(\cos(\omega_Mt),\sin(\omega_Mt))" />
</p>

The apparent position of Mars from Earth is:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?\vec{r}_{M/Z}(t)=\vec{r}_M(t)-\vec{r}_Z(t)" />
</p>

Retrograde motion occurs when Earth overtakes Mars in its orbit. Therefore, retrograde loops do not require epicycles; they are a natural result of observing Mars from a moving Earth.
