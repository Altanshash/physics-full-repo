# Problem 3 – Comparison of Models: Number of Parameters and Quality of Description

## Given

We compare two models of planetary motion:

1. The epicycle model.
2. The heliocentric model.

The goal is to fit the epicycle parameters to the trajectory generated in the heliocentric model.

The epicycle model can be written as:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x(t)=R\cos(\omega t)+r\cos(\Omega t)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y(t)=R\sin(\omega t)+r\sin(\Omega t)" />
</p>

The heliocentric relative trajectory can be written as:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x(t)=R_M\cos(\omega_Mt)-R_Z\cos(\omega_Zt)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y(t)=R_M\sin(\omega_Mt)-R_Z\sin(\omega_Zt)" />
</p>

---

## Solution

## 1. Fitting the Epicycle Parameters

To make the epicycle model match the heliocentric relative trajectory, we compare the two forms.

Epicycle model:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x(t)=R\cos(\omega t)+r\cos(\Omega t)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y(t)=R\sin(\omega t)+r\sin(\Omega t)" />
</p>

Heliocentric relative model:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?x(t)=R_M\cos(\omega_Mt)-R_Z\cos(\omega_Zt)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?y(t)=R_M\sin(\omega_Mt)-R_Z\sin(\omega_Zt)" />
</p>

The negative term can be written as a phase shift:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?-R_Z\cos(\omega_Zt)=R_Z\cos(\omega_Zt+\pi)" />
</p>

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?-R_Z\sin(\omega_Zt)=R_Z\sin(\omega_Zt+\pi)" />
</p>

So the heliocentric relative trajectory has the same mathematical structure as an epicycle model.

A possible correspondence is:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?R=R_M,\quad r=R_Z,\quad \omega=\omega_M,\quad \Omega=\omega_Z" />
</p>

with a phase shift of π for the Earth-related term.

---

## 2. Number of Parameters in Both Models

The basic epicycle model uses the following parameters:

- Radius of deferent: **R**
- Radius of epicycle: **r**
- Angular velocity of deferent: **ω**
- Angular velocity of epicycle: **Ω**

So the epicycle model has **4 main parameters**.

The heliocentric model uses:

- Earth orbit radius: **RZ**
- Mars orbit radius: **RM**
- Earth angular velocity: **ωZ**
- Mars angular velocity: **ωM**

So the heliocentric model also has **4 main parameters** for two circular orbits.

However, the interpretation is different.

In the epicycle model, parameters are introduced to reproduce the apparent motion.

In the heliocentric model, parameters describe real orbital motion around the Sun.

---

## 3. Which Model Is More Economical?

Both models can reproduce similar retrograde loops.

However, the heliocentric model is more economical because:

- It explains retrograde motion naturally.
- It does not need artificial epicycles.
- The same principle explains the motion of different planets.
- Retrograde motion appears because Earth overtakes Mars.

The epicycle model can fit observations, but it becomes more complicated when higher accuracy is needed.

---

## 4. Interpretation

The comparison shows that two models can sometimes describe the same observed trajectory.

The epicycle model is mathematically useful, but it treats retrograde motion as an added geometric construction.

The heliocentric model gives a simpler physical explanation. It explains the same phenomenon as a result of relative motion.

Thus, the heliocentric model simplifies the description of planetary motion.

---

# Conclusion

The epicycle model and the heliocentric model can produce similar apparent trajectories.

The epicycle parameters can be fitted to the heliocentric trajectory by matching:

<p align="center">
  <img src="https://latex.codecogs.com/svg.image?R=R_M,\quad r=R_Z,\quad \omega=\omega_M,\quad \Omega=\omega_Z" />
</p>

with a phase shift of π.

Although both models may use a similar number of basic parameters, the heliocentric model is more economical in meaning.

It explains retrograde motion as a natural consequence of relative motion, while the epicycle model introduces extra circular motion to reproduce the same effect.

Therefore, the heliocentric model gives a simpler and more physically meaningful description of planetary motion.
