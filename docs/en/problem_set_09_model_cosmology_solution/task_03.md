# Problem 3 – Comparison of Models: Number of Parameters and Quality of Description

## Given

We compare two models of planetary motion:

1. The epicycle model.
2. The heliocentric model.

The epicycle model is:

$$
x(t)=R\cos(\omega t)+r\cos(\Omega t)
$$

$$
y(t)=R\sin(\omega t)+r\sin(\Omega t)
$$

The heliocentric relative trajectory is:

$$
x(t)=R_M\cos(\omega_M t)-R_Z\cos(\omega_Z t)
$$

$$
y(t)=R_M\sin(\omega_M t)-R_Z\sin(\omega_Z t)
$$

---

## Solution

### 1. Fitting the Epicycle Parameters

The epicycle model and the heliocentric relative model have similar forms.

Epicycle model:

$$
x(t)=R\cos(\omega t)+r\cos(\Omega t)
$$

$$
y(t)=R\sin(\omega t)+r\sin(\Omega t)
$$

Heliocentric relative model:

$$
x(t)=R_M\cos(\omega_M t)-R_Z\cos(\omega_Z t)
$$

$$
y(t)=R_M\sin(\omega_M t)-R_Z\sin(\omega_Z t)
$$

The negative terms can be interpreted as a phase shift of pi:

$$
-R_Z\cos(\omega_Z t)=R_Z\cos(\omega_Z t+\pi)
$$

$$
-R_Z\sin(\omega_Z t)=R_Z\sin(\omega_Z t+\pi)
$$

Therefore, the parameters can be matched as:

$$
R=R_M
$$

$$
r=R_Z
$$

$$
\omega=\omega_M
$$

$$
\Omega=\omega_Z
$$

with a phase shift of pi for the Earth term.

---

### 2. Number of Parameters in Both Models

The basic epicycle model uses four main parameters:

- Radius of deferent: $R$
- Radius of epicycle: $r$
- Angular velocity of deferent: $\omega$
- Angular velocity of epicycle: $\Omega$

So the epicycle model has **4 main parameters**.

The heliocentric model also uses four main parameters:

- Earth orbit radius: $R_Z$
- Mars orbit radius: $R_M$
- Earth angular velocity: $\omega_Z$
- Mars angular velocity: $\omega_M$

So the heliocentric model also has **4 main parameters**.

However, their meanings are different. In the epicycle model, parameters are used mainly to reproduce the observed motion. In the heliocentric model, parameters describe real circular motion around the Sun.

---

### 3. Which Model Is More Economical?

Both models can reproduce a similar retrograde loop.

However, the heliocentric model is more economical because retrograde motion appears naturally from relative motion.

Earth moves on an inner orbit and has a larger angular velocity. When Earth overtakes Mars, Mars appears to move backward in the sky.

The epicycle model can describe this motion, but it needs an additional circular motion to explain the loop.

---

### 4. Interpretation

This comparison shows that different mathematical models can describe the same observed motion.

The epicycle model is useful for fitting the apparent trajectory, but it does not give a simple physical explanation.

The heliocentric model explains the same effect more naturally. Retrograde motion is not a separate special motion; it is the result of observing Mars from a moving Earth.

---

## Conclusion

The epicycle model and the heliocentric model can produce similar apparent trajectories.

A simple parameter correspondence is:

$$
R=R_M
$$

$$
r=R_Z
$$

$$
\omega=\omega_M
$$

$$
\Omega=\omega_Z
$$

with a phase shift of pi.

Although both models use four main parameters, the heliocentric model is more economical because it explains retrograde motion naturally.

Therefore, the heliocentric model gives a simpler and more physically meaningful description of planetary motion.
