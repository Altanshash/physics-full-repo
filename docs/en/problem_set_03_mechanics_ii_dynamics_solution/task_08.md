## Problem 8 – Harmonic oscillator (formal dynamics)

### Problem statement

We consider the equation

$$
m\ddot{x} + kx = 0
$$

Determine:

- the solution,
- the natural frequency,
- the energy,
- show that energy is conserved,
- interpret the motion in phase space.

---

## Solution

### 1. Rewrite the equation

Divide by $m$:

$$
\ddot{x} + \frac{k}{m}x = 0
$$

Introduce

$$
\omega_0^2 = \frac{k}{m}
$$

Then

$$
\ddot{x} + \omega_0^2 x = 0
$$

---

### 2. Solve the equation

The standard solution of

$$
\ddot{x} + \omega_0^2 x = 0
$$

is

$$
x(t) = A\cos(\omega_0 t) + B\sin(\omega_0 t)
$$

So,

$$
\boxed{x(t) = A\cos(\omega_0 t) + B\sin(\omega_0 t)}
$$

---

### 3. Natural frequency

From

$$
\omega_0^2 = \frac{k}{m}
$$

we get

$$
\boxed{\omega_0 = \sqrt{\frac{k}{m}}}
$$

The period is

$$
\boxed{T = \frac{2\pi}{\omega_0} = 2\pi\sqrt{\frac{m}{k}}}
$$

---

### 4. Velocity

Differentiate $x(t)$:

$$
\dot{x}(t) = -A\omega_0\sin(\omega_0 t) + B\omega_0\cos(\omega_0 t)
$$

Thus,

$$
\boxed{\dot{x}(t) = -A\omega_0\sin(\omega_0 t) + B\omega_0\cos(\omega_0 t)}
$$

---

### 5. Energy

The total energy is

$$
E(t) = \frac{1}{2}m\dot{x}^2 + \frac{1}{2}kx^2
$$

So,

$$
\boxed{E(t) = \frac{1}{2}m\dot{x}^2 + \frac{1}{2}kx^2}
$$

---

### 6. Show that energy is conserved

Differentiate the energy:

$$
\frac{dE}{dt} = m\dot{x}\ddot{x} + kx\dot{x}
$$

Factor out $\dot{x}$:

$$
\frac{dE}{dt} = \dot{x}(m\ddot{x} + kx)
$$

But from the equation of motion,

$$
m\ddot{x} + kx = 0
$$

Therefore,

$$
\frac{dE}{dt} = 0
$$

Hence,

$$
\boxed{E = \text{constant}}
$$

So the energy is conserved.

---

### 7. Phase space interpretation

In phase space, the motion is described by $(x,\dot{x})$.

For the harmonic oscillator, the trajectory is a closed curve.  
Using the energy equation,

$$
\frac{1}{2}m\dot{x}^2 + \frac{1}{2}kx^2 = E
$$

we can rewrite it as

$$
\frac{k}{2}x^2 + \frac{m}{2}\dot{x}^2 = E
$$

This is the equation of an ellipse in the $(x,\dot{x})$ plane.

So the phase trajectory is closed, which means the motion is periodic.

---

## Conclusion

The solution is

$$
\boxed{x(t) = A\cos(\omega_0 t) + B\sin(\omega_0 t)}
$$

with

$$
\boxed{\omega_0 = \sqrt{\frac{k}{m}}}
$$

The energy is

$$
\boxed{E(t) = \frac{1}{2}m\dot{x}^2 + \frac{1}{2}kx^2}
$$

and it is conserved:

$$
\boxed{\frac{dE}{dt} = 0}
$$

In phase space, the motion is represented by an ellipse.
