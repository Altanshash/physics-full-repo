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

### 1. General form of the solution

The total solution of the forced oscillator is the sum of:

1. the **homogeneous solution** $x_h(t)$  
2. the **particular solution** $x_p(t)$  

So,

$$
x(t) = x_h(t) + x_p(t)
$$

The homogeneous part describes the transient motion.  
The particular part describes the steady-state forced motion.

---

### 2. Homogeneous solution

First, solve the homogeneous equation:

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0
$$

Assume a solution of the form

$$
x_h(t) = e^{rt}
$$

Then

$$
\frac{dx_h}{dt} = re^{rt}
$$

and

$$
\frac{d^2x_h}{dt^2} = r^2e^{rt}
$$

Substitute into the homogeneous equation:

$$
mr^2e^{rt} + bre^{rt} + ke^{rt} = 0
$$

Factor out $e^{rt}$:

$$
e^{rt}(mr^2 + br + k) = 0
$$

Since $e^{rt} \neq 0$, we get the characteristic equation

$$
mr^2 + br + k = 0
$$

The roots are

$$
r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}
$$

So the homogeneous solution is the same as in the damped oscillator problem.

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

Substitute into the equation

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = F_0\cos(\Omega t)
$$

Then

$$
m\left(-C\Omega^2\cos(\Omega t) - D\Omega^2\sin(\Omega t)\right)
+ b\left(-C\Omega\sin(\Omega t) + D\Omega\cos(\Omega t)\right)
+ k\left(C\cos(\Omega t) + D\sin(\Omega t)\right)
= F_0\cos(\Omega t)
$$

Now group the terms with $\cos(\Omega t)$ and $\sin(\Omega t)$.

For $\cos(\Omega t)$:

$$
\left[(k - m\Omega^2)C + b\Omega D\right]\cos(\Omega t)
$$

For $\sin(\Omega t)$:

$$
\left[(k - m\Omega^2)D - b\Omega C\right]\sin(\Omega t)
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

The steady-state solution can be written in the form

$$
x_p(t) = A(\Omega)\cos(\Omega t - \phi)
$$

where $A(\Omega)$ is the amplitude and $\phi$ is the phase shift.

From the system of equations, the amplitude is

$$
\boxed{
A(\Omega) = \frac{F_0}{\sqrt{(k - m\Omega^2)^2 + (b\Omega)^2}}
}
$$

This is the required amplitude as a function of $\Omega$.

---

### 5. Phase shift

The phase shift is determined by

$$
\boxed{
\tan\phi = \frac{b\Omega}{k - m\Omega^2}
}
$$

Therefore,

$$
\boxed{
\phi = \arctan\left(\frac{b\Omega}{k - m\Omega^2}\right)
}
$$

Interpretation:

- when $\Omega$ is small, $\phi \approx 0$
- near resonance, $\phi \approx \frac{\pi}{2}$
- when $\Omega$ is large, $\phi \to \pi$

---

### 6. Resonance condition

The natural frequency of the undamped oscillator is

$$
\omega_0 = \sqrt{\frac{k}{m}}
$$

Resonance occurs when the forcing frequency $\Omega$ is close to the natural frequency:

$$
\Omega \approx \omega_0
$$

In that case, the denominator in the amplitude formula becomes small, so the amplitude becomes large.

If damping is present, the resonance peak is finite.

---

### 7. Numerical solution

To solve the equation numerically, convert it into a system of first-order equations.

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

So the system becomes

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

This system can be solved numerically using the Runge–Kutta 4th order method (RK4).

---

### 8. Resonance curve

The resonance curve is the graph of steady-state amplitude versus forcing frequency:

$$
A(\Omega) \text{ versus } \Omega
$$

Using the formula

$$
A(\Omega) = \frac{F_0}{\sqrt{(k - m\Omega^2)^2 + (b\Omega)^2}}
$$

we observe:

1. for small $\Omega$, the amplitude is small  
2. near resonance, the amplitude reaches a maximum  
3. for large $\Omega$, the amplitude decreases again  

If damping $b$ increases:

- the resonance peak becomes lower
- the resonance curve becomes wider
- the system becomes less sensitive to resonance

---

### 9. Physical interpretation of resonance

The external force continuously gives energy to the oscillator.

If the forcing frequency is far from the natural frequency, the energy transfer is weak, so the amplitude remains small.

If the forcing frequency is close to the natural frequency, the energy transfer is most efficient, so the amplitude becomes large.

This phenomenon is called **resonance**.

Damping removes energy from the system, so it limits the amplitude and prevents infinite growth.

---

## Final Answer

The forced damped oscillator

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = F_0\cos(\Omega t)
$$

has a steady-state solution of the form

$$
\boxed{
x_p(t) = A(\Omega)\cos(\Omega t - \phi)
}
$$

where the amplitude is

$$
\boxed{
A(\Omega) = \frac{F_0}{\sqrt{(k - m\Omega^2)^2 + (b\Omega)^2}}
}
$$

and the phase shift is

$$
\boxed{
\tan\phi = \frac{b\Omega}{k - m\Omega^2}
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
\frac{dv}{dt} = \frac{1}{m}\left(F_0\cos(\Omega t) - bv - kx\right)
}
$$

The resonance curve is obtained by plotting

$$
A(\Omega) \text{ versus } \Omega
$$

---

## Conclusion

The forced oscillator shows resonance when the forcing frequency is close to the natural frequency.

The oscillation amplitude is

$$
\boxed{
A(\Omega) = \frac{F_0}{\sqrt{(k - m\Omega^2)^2 + (b\Omega)^2}}
}
$$

and the phase shift changes with frequency according to

$$
\boxed{
\tan\phi = \frac{b\Omega}{k - m\Omega^2}
}
$$

Damping reduces the resonance peak and prevents unlimited growth of amplitude.
