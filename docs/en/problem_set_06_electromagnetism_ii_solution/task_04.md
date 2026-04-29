# Problem 4 – Rotating Loop (Induction)

## Problem Statement

A loop with area $S$ and $N$ turns is placed in a uniform magnetic field $\vec{B}$.

The loop rotates with angular velocity $\omega$ around an axis perpendicular to $\vec{B}$.

Answer the following questions:

1. Determine $\Phi(t)$.
2. Determine $\mathcal{E}(t)$.
3. Calculate the amplitude $\mathcal{E}_0$.
4. How does the amplitude depend on $\omega$?
5. Interpret the mechanism of EMF generation.

---

## Given

$$
S = \text{area of the loop}
$$

$$
N = \text{number of turns}
$$

$$
\vec{B} = \text{uniform magnetic field}
$$

$$
\omega = \text{angular velocity}
$$

$$
\theta = \omega t
$$

---

## Solution

## 1. Magnetic Flux

Magnetic flux through one loop is:

$$
\Phi(t) = BS\cos\theta
$$

Since the loop rotates:

$$
\theta = \omega t
$$

Therefore:

$$
\Phi(t) = BS\cos(\omega t)
$$

For $N$ turns:

$$
\Phi_N(t) = NBS\cos(\omega t)
$$

---

## 2. Induced EMF

According to Faraday's law:

$$
\mathcal{E}(t) = -\frac{d\Phi_N(t)}{dt}
$$

Substitute:

$$
\mathcal{E}(t) = -\frac{d}{dt}\left(NBS\cos(\omega t)\right)
$$

Differentiate:

$$
\mathcal{E}(t) = NBS\omega \sin(\omega t)
$$

---

## 3. EMF Amplitude

The amplitude is the maximum value of EMF.

Since:

$$
\mathcal{E}(t) = NBS\omega \sin(\omega t)
$$

and:

$$
\sin(\omega t)_{\max} = 1
$$

then:

$$
\mathcal{E}_0 = NBS\omega
$$

---

## 4. Dependence on Angular Velocity

The amplitude is:

$$
\mathcal{E}_0 = NBS\omega
$$

So:

$$
\mathcal{E}_0 \propto \omega
$$

This means if angular velocity increases, the EMF amplitude also increases.

For example:

$$
\omega \rightarrow 2\omega
$$

then:

$$
\mathcal{E}_0 \rightarrow 2\mathcal{E}_0
$$

---

## 5. Mechanism of EMF Generation

When the loop rotates in a magnetic field, the angle between the loop normal and the magnetic field changes with time.

Because of this, the magnetic flux changes:

$$
\Phi(t) = NBS\cos(\omega t)
$$

A changing magnetic flux produces an induced EMF:

$$
\mathcal{E}(t) = -\frac{d\Phi}{dt}
$$

This is the basic principle of an electric generator.

---

## Final Conclusion

The magnetic flux is:

$$
\Phi(t) = NBS\cos(\omega t)
$$

The induced EMF is:

$$
\mathcal{E}(t) = NBS\omega\sin(\omega t)
$$

The amplitude of EMF is:

$$
\mathcal{E}_0 = NBS\omega
$$

The amplitude is directly proportional to angular velocity:

$$
\mathcal{E}_0 \propto \omega
$$

A rotating loop generates EMF because the magnetic flux through the loop changes with time.
