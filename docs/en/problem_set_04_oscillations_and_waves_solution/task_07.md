# Problem 7 – Forced oscillator and resonance

## Given

The equation is

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = F_0\cos(\Omega t)
$$

We need to:

1. Solve the equation analytically and determine the amplitude as a function of $\Omega$.
2. Solve the equation numerically.
3. Investigate the steady-state amplitude as a function of $\Omega$.
4. Generate the resonance curve.
5. Investigate the phase shift.
6. Interpret the phenomenon of resonance.

---

## Solution

### 1. General form of the solution

The total solution is the sum of the homogeneous solution and the particular solution:

$$
x(t) = x_h(t) + x_p(t)
$$

The homogeneous part describes the transient motion, and the particular part describes the steady-state forced motion.

---

### 2. Homogeneous solution

First solve the homogeneous equation:

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0
$$

Assume

$$
x_h(t) = e^{rt}
$$

Then

$$
\frac{dx_h}{dt} = re^{rt}
$$

$$
\frac{d^2x_h}{dt^2} = r^2 e^{rt}
$$

Substitute into the equation:

$$
mr^2 e^{rt} + br e^{rt} + k e^{rt} = 0
$$

Factor out $e^{rt}$:

$$
e^{rt}(mr^2 + br + k) = 0
$$

Since $e^{rt} \ne 0$, the characteristic equation is

$$
mr^2 + br + k = 0
$$

The roots are

$$
r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}
$$

So the homogeneous solution is the same as for the damped oscillator.

---

### 3. Particular solution

Assume a particular solution of the form

$$
x_p(t) = C\cos(\Omega t) + D\sin(\Omega t)
$$

First derivative:

$$
\frac{dx_p}{dt} = -C\Omega\sin(\Omega t) + D\Omega\cos(\Omega t)
$$

Second derivative:

$$
\frac{d^2x_p}{dt^2} = -C\Omega^2\cos(\Omega t) - D\Omega^2\sin(\Omega t)
$$

Substitute into the original equation:

$$
m\left(-C\Omega^2\cos(\Omega t) - D\Omega^2\sin(\Omega t)\right) + b\left(-C\Omega\sin(\Omega t) + D\Omega\cos(\Omega t)\right) + k\left(C\cos(\Omega t) + D\sin(\Omega t)\right) = F_0\cos(\Omega t)
$$

Now collect the coefficients of $\cos(\Omega t)$ and $\sin(\Omega t)$.

For $\cos(\Omega t)$:

$$
(k - m\Omega^2)C + b\Omega D
$$

For $\sin(\Omega t)$:

$$
(k - m\Omega^2)D - b\Omega C
$$

Therefore, we obtain the system

$$
(k - m\Omega^2)C + b\Omega D = F_0
$$

$$
(k - m\Omega^2)D - b\Omega C = 0
$$

---

### 4. Amplitude of oscillations

The steady-state solution can be written as

$$
x_p(t) = A(\Omega)\cos(\Omega t - \phi)
$$

where $A(\Omega)$ is the amplitude and $\phi$ is the phase shift.

The amplitude is

$$
\boxed{A(\Omega) = \frac{F_0}{\sqrt{(k - m\Omega^2)^2 + (b\Omega)^2}}}
$$

This is the amplitude as a function of $\Omega$.

---

### 5. Phase shift

The phase shift satisfies

$$
\boxed{\tan\phi = \frac{b\Omega}{k - m\Omega^2}}
$$

Hence,

$$
\boxed{\phi = \arctan\left(\frac{b\Omega}{k - m\Omega^2}\right)}
$$

Interpretation:

- for small $\Omega$, the phase shift is close to $0$
- near resonance, the phase shift is close to $\frac{\pi}{2}$
- for large $\Omega$, the phase shift approaches $\pi$

---

### 6. Resonance condition

The natural frequency of the undamped oscillator is

$$
\omega_0 = \sqrt{\frac{k}{m}}
$$

Resonance occurs when the forcing frequency is close to the natural frequency:

$$
\Omega \approx \omega_0
$$

In this case the amplitude becomes large.

If damping is present, the resonance peak is finite.

---

### 7. Numerical solution

To solve the equation numerically, convert it into a first-order system.

Let

$$
v = \frac{dx}{dt}
$$

Then

$$
\frac{dx}{dt} = v
$$

$$
\frac{dv}{dt} = \frac{1}{m}\left(F_0\cos(\Omega t) - bv - kx\right)
$$

So the numerical system is

$$
\boxed{\frac{dx}{dt} = v}
$$

$$
\boxed{\frac{dv}{dt} = \frac{1}{m}\left(F_0\cos(\Omega t) - bv - kx\right)}
$$

This system can be solved by the RK4 method.

---

### 8. Resonance curve

The resonance curve is the graph of steady-state amplitude versus forcing frequency:

$$
A(\Omega) \text{ versus } \Omega
$$

Using

$$
A(\Omega) = \frac{F_0}{\sqrt{(k - m\Omega^2)^2 + (b\Omega)^2}}
$$

we see:

1. for small $\Omega$, the amplitude is small
2. near resonance, the amplitude reaches a maximum
3. for large $\Omega$, the amplitude decreases again

If damping $b$ increases:

- the peak becomes lower
- the curve becomes wider
- resonance becomes less sharp

---

### 9. Physical interpretation

The external force continuously transfers energy to the oscillator.

- If the forcing frequency is far from the natural frequency, the response is small.
- If the forcing frequency is close to the natural frequency, energy transfer is most efficient.
- Then the amplitude becomes large. This is resonance.

Damping removes energy from the system, so it limits the amplitude.

---

## Final Answer

The forced damped oscillator

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = F_0\cos(\Omega t)
$$

has the steady-state solution

$$
\boxed{x_p(t) = A(\Omega)\cos(\Omega t - \phi)}
$$

with amplitude

$$
\boxed{A(\Omega) = \frac{F_0}{\sqrt{(k - m\Omega^2)^2 + (b\Omega)^2}}}
$$

and phase shift

$$
\boxed{\tan\phi = \frac{b\Omega}{k - m\Omega^2}}
$$

The numerical system is

$$
\boxed{\frac{dx}{dt} = v}
$$

$$
\boxed{\frac{dv}{dt} = \frac{1}{m}\left(F_0\cos(\Omega t) - bv - kx\right)}
$$

The resonance curve is obtained by plotting $A(\Omega)$ as a function of $\Omega$.

---

## Conclusion

The forced oscillator shows resonance when the forcing frequency is close to the natural frequency.

The amplitude is

$$
\boxed{A(\Omega) = \frac{F_0}{\sqrt{(k - m\Omega^2)^2 + (b\Omega)^2}}}
$$

and the phase shift is determined by

$$
\boxed{\tan\phi = \frac{b\Omega}{k - m\Omega^2}}
$$

Damping reduces the resonance peak and prevents unlimited growth of amplitude.
