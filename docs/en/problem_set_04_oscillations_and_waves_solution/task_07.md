# Problem 7 – Forced oscillator and resonance

## Given

The equation is

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = F_0\cos(\Omega t)
$$

We need to:

1. Solve the equation analytically and determine the amplitude of oscillations as a function of $\Omega$.
2. Solve the equation numerically.
3. Investigate the steady-state amplitude as a function of $\Omega$.
4. Generate the resonance curve.
5. Investigate the phase shift.
6. Interpret the phenomenon of resonance.

---

## Solution

### 1. Analytical solution

The equation of motion is

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = F_0\cos(\Omega t)
$$

The total solution is the sum of:

1. the **homogeneous solution** $x_h(t)$
2. the **particular solution** $x_p(t)$

So,

$$
x(t) = x_h(t) + x_p(t)
$$

---

### 2. Homogeneous solution

The homogeneous equation is

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0
$$

Its characteristic equation is

$$
mr^2 + br + k = 0
$$

The roots are

$$
r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}
$$

So the transient part of motion is the same as for the damped oscillator:

- **Underdamped**: oscillatory decay
- **Critically damped**: fastest non-oscillatory decay
- **Overdamped**: slow non-oscillatory decay

This part disappears with time because of damping.

---

### 3. Particular solution

To find the steady-state solution, assume

$$
x_p(t) = C\cos(\Omega t) + D\sin(\Omega t)
$$

Then

$$
\frac{dx_p}{dt} = -C\Omega\sin(\Omega t) + D\Omega\cos(\Omega t)
$$

$$
\frac{d^2x_p}{dt^2} = -C\Omega^2\cos(\Omega t) - D\Omega^2\sin(\Omega t)
$$

Substitute into the equation:

$$
m(-C\Omega^2\cos(\Omega t) - D\Omega^2\sin(\Omega t))
+ b(-C\Omega\sin(\Omega t) + D\Omega\cos(\Omega t))
+ k(C\cos(\Omega t) + D\sin(\Omega t))
= F_0\cos(\Omega t)
$$

Group the cosine terms:

$$
(k - m\Omega^2)C + b\Omega D
$$

Group the sine terms:

$$
(k - m\Omega^2)D - b\Omega C
$$

Therefore, we obtain the system:

$$
(k - m\Omega^2)C + b\Omega D = F_0
$$

$$
(k - m\Omega^2)D - b\Omega C = 0
$$

---

### 4. Amplitude as a function of $\Omega$

The steady-state solution can be written in the form

$$
x_p(t) = A(\Omega)\cos(\Omega t - \phi)
$$

where the amplitude is

$$
\boxed{
A(\Omega)=\frac{F_0}{\sqrt{(k-m\Omega^2)^2 + (b\Omega)^2}}
}
$$

This is the amplitude-frequency relation.

It shows how the oscillation amplitude depends on the forcing frequency $\Omega$.

---

### 5. Phase shift

The phase shift between the external force and the oscillation is

$$
\boxed{
\tan\phi = \frac{b\Omega}{k-m\Omega^2}
}
$$

Thus,

$$
\boxed{
\phi = \arctan\left(\frac{b\Omega}{k-m\Omega^2}\right)
}
$$

Interpretation:

- for small $\Omega$, the phase shift is close to $0$
- near resonance, the phase shift is close to $\frac{\pi}{2}$
- for large $\Omega$, the phase shift approaches $\pi$

---

### 6. Resonance

If damping is small, the amplitude becomes very large when the forcing frequency is close to the natural frequency.

The natural frequency of the undamped oscillator is

$$
\omega_0 = \sqrt{\frac{k}{m}}
$$

Resonance occurs near

$$
\Omega \approx \omega_0
$$

When damping is present, the resonance peak is finite and slightly shifted.

So the resonance curve is the graph of

$$
A(\Omega)=\frac{F_0}{\sqrt{(k-m\Omega^2)^2 + (b\Omega)^2}}
$$

as a function of $\Omega$.

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

and

$$
\frac{dv}{dt} = \frac{1}{m}\left(F_0\cos(\Omega t) - bv - kx\right)
$$

So the system is

$$
\boxed{
\frac{dx}{dt} = v
}
$$

$$
\boxed{
\frac{dv}{dt} = \frac{1}{m}\left(F_0\cos(\Omega t) - bv - kx\right)
}
$$

This system can be solved numerically using RK4.

For each forcing frequency $\Omega$, we can compute the trajectory $x(t)$ and then measure the steady-state amplitude.

---

### 8. Resonance curve

The resonance curve is the graph of steady-state amplitude versus forcing frequency.

That is,

$$
A(\Omega) \text{ versus } \Omega
$$

Properties:

- small amplitude for very low frequency
- maximum amplitude near resonance
- smaller amplitude again for high frequency

If damping $b$ increases:

- the peak becomes lower
- the curve becomes wider
- resonance becomes less sharp

---

### 9. Physical interpretation

The external force continuously supplies energy to the oscillator.

- If the forcing frequency is far from the natural frequency, the response is weak.
- If the forcing frequency is close to the natural frequency, energy transfer is most efficient.
- Then the oscillation amplitude becomes large: this is **resonance**.

Damping removes energy, so it limits the amplitude.

That is why real systems do not have infinite amplitude at resonance.

---

## Final Answer

The forced damped oscillator

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = F_0\cos(\Omega t)
$$

has a steady-state solution of the form

$$
\boxed{
x_p(t)=A(\Omega)\cos(\Omega t-\phi)
}
$$

with amplitude

$$
\boxed{
A(\Omega)=\frac{F_0}{\sqrt{(k-m\Omega^2)^2 + (b\Omega)^2}}
}
$$

and phase shift

$$
\boxed{
\tan\phi = \frac{b\Omega}{k-m\Omega^2}
}
$$

The numerical system is

$$
\boxed{
\frac{dx}{dt} = v
}
$$

$$
\boxed{
\frac{dv}{dt} = \frac{1}{m}\left(F_0\cos(\Omega t)-bv-kx\right)
}
$$

The resonance curve is obtained by plotting $A(\Omega)$ versus $\Omega$.

---

## Conclusion

The forced oscillator shows resonance when the forcing frequency is close to the natural frequency.  
The oscillation amplitude is determined by the function

$$
A(\Omega)=\frac{F_0}{\sqrt{(k-m\Omega^2)^2 + (b\Omega)^2}}
$$

and the phase shift changes from approximately $0$ to $\pi$ as the forcing frequency increases.  
Damping reduces the resonance peak and prevents unlimited growth of amplitude.
