## Problem 8 – Harmonic oscillator (formal dynamics)

### Problem statement

We consider the equation of motion

$$
m\ddot{x} + kx = 0
$$

Determine:

- solve the equation,
- determine the natural frequency,
- write down the energy as a function of time,
- show that energy is conserved,
- interpret the motion in phase space.

---

## Solution

### 1. Differential equation

The given equation is

$$
m\ddot{x} + kx = 0
$$

Divide both sides by $m$:

$$
\ddot{x} + \frac{k}{m}x = 0
$$

Introduce the notation

$$
\omega_0^2 = \frac{k}{m}
$$

Then the equation becomes

$$
\ddot{x} + \omega_0^2 x = 0
$$

This is the standard equation of a harmonic oscillator.

---

### 2. General solution

We look for a solution of the form

$$
x(t) = e^{\lambda t}
$$

Then

$$
\dot{x}(t) = \lambda e^{\lambda t},
\qquad
\ddot{x}(t) = \lambda^2 e^{\lambda t}
$$

Substitute into the differential equation:

$$
\lambda^2 e^{\lambda t} + \omega_0^2 e^{\lambda t} = 0
$$

Since $e^{\lambda t} \neq 0$, we get the characteristic equation

$$
\lambda^2 + \omega_0^2 = 0
$$

So the roots are

$$
\lambda = \pm i\omega_0
$$

Therefore, the general real solution is

$$
\boxed{
x(t) = A\cos(\omega_0 t) + B\sin(\omega_0 t)
}
$$

where $A$ and $B$ are constants determined by the initial conditions.

An equivalent form is

$$
\boxed{
x(t) = C\cos(\omega_0 t + \varphi)
}
$$

where $C$ is the amplitude and $\varphi$ is the phase constant.

---

### 3. Natural frequency

From

$$
\omega_0^2 = \frac{k}{m}
$$

we obtain the natural angular frequency

$$
\boxed{
\omega_0 = \sqrt{\frac{k}{m}}
}
$$

The ordinary frequency is

$$
\boxed{
f = \frac{\omega_0}{2\pi} = \frac{1}{2\pi}\sqrt{\frac{k}{m}}
}
$$

and the period is

$$
\boxed{
T = \frac{2\pi}{\omega_0} = 2\pi\sqrt{\frac{m}{k}}
}
$$

---

### 4. Velocity

Differentiate the position:

$$
x(t) = A\cos(\omega_0 t) + B\sin(\omega_0 t)
$$

Then

$$
\dot{x}(t) = -A\omega_0\sin(\omega_0 t) + B\omega_0\cos(\omega_0 t)
$$

So the velocity is

$$
\boxed{
v(t) = \dot{x}(t) = -A\omega_0\sin(\omega_0 t) + B\omega_0\cos(\omega_0 t)
}
$$

If we use the form $x(t)=C\cos(\omega_0 t+\varphi)$, then

$$
\boxed{
v(t) = -C\omega_0\sin(\omega_0 t+\varphi)
}
$$

---

### 5. Energy as a function of time

The total mechanical energy is the sum of kinetic and potential energy:

$$
E(t) = T(t) + U(t)
$$

The kinetic energy is

$$
T(t) = \frac{1}{2}m\dot{x}^2
$$

The potential energy is

$$
U(t) = \frac{1}{2}kx^2
$$

Therefore,

$$
\boxed{
E(t) = \frac{1}{2}m\dot{x}^2 + \frac{1}{2}kx^2
}
$$

Using the form

$$
x(t) = C\cos(\omega_0 t+\varphi),
\qquad
\dot{x}(t) = -C\omega_0\sin(\omega_0 t+\varphi)
$$

we get

$$
E(t)
=
\frac{1}{2}mC^2\omega_0^2\sin^2(\omega_0 t+\varphi)
+
\frac{1}{2}kC^2\cos^2(\omega_0 t+\varphi)
$$

Since

$$
\omega_0^2 = \frac{k}{m}
$$

it follows that

$$
m\omega_0^2 = k
$$

So the energy becomes

$$
E(t)
=
\frac{1}{2}kC^2\sin^2(\omega_0 t+\varphi)
+
\frac{1}{2}kC^2\cos^2(\omega_0 t+\varphi)
$$

Factor out $\frac{1}{2}kC^2$:

$$
E(t)
=
\frac{1}{2}kC^2
\left[
\sin^2(\omega_0 t+\varphi) + \cos^2(\omega_0 t+\varphi)
\right]
$$

Using

$$
\sin^2\theta + \cos^2\theta = 1
$$

we obtain

$$
\boxed{
E(t) = \frac{1}{2}kC^2
}
$$

So the total energy does not depend on time.

---

### 6. Proof that energy is conserved

From the previous result,

$$
E(t) = \frac{1}{2}kC^2
$$

which is constant.

Therefore,

$$
\boxed{
\frac{dE}{dt} = 0
}
$$

Hence, the total mechanical energy is conserved.

This means that energy continuously changes form between kinetic and potential energy, but the total remains the same.

---

### 7. Phase space interpretation

In phase space, the motion is described by the pair

$$
(x,v)
$$

For the harmonic oscillator,

$$
x(t) = C\cos(\omega_0 t+\varphi)
$$

$$
v(t) = -C\omega_0\sin(\omega_0 t+\varphi)
$$

Divide the first equation by $C$:

$$
\frac{x}{C} = \cos(\omega_0 t+\varphi)
$$

Divide the second equation by $C\omega_0$:

$$
\frac{v}{C\omega_0} = -\sin(\omega_0 t+\varphi)
$$

Now square both equations and add them:

$$
\frac{x^2}{C^2} + \frac{v^2}{C^2\omega_0^2}
=
\cos^2(\omega_0 t+\varphi) + \sin^2(\omega_0 t+\varphi)
= 1
$$

Therefore, the phase trajectory is

$$
\boxed{
\frac{x^2}{C^2} + \frac{v^2}{C^2\omega_0^2} = 1
}
$$

This is an ellipse in the $(x,v)$ plane.

So in phase space:

- the oscillator moves along a closed curve,
- the motion is periodic,
- each energy value corresponds to one ellipse.

---

## Conclusion

The harmonic oscillator satisfies the equation

$$
m\ddot{x} + kx = 0
$$

Its solution is

$$
\boxed{
x(t) = A\cos(\omega_0 t) + B\sin(\omega_0 t)
}
$$

with natural angular frequency

$$
\boxed{
\omega_0 = \sqrt{\frac{k}{m}}
}
$$

The total mechanical energy is

$$
\boxed{
E(t) = \frac{1}{2}m\dot{x}^2 + \frac{1}{2}kx^2 = \frac{1}{2}kC^2
}
$$

So the energy is conserved.

In phase space, the motion is represented by the ellipse

$$
\boxed{
\frac{x^2}{C^2} + \frac{v^2}{C^2\omega_0^2} = 1
}
$$
