# Problem 4 – Wave equation

## Given

The function is:

$$
y(x,t) = A \cos(kx - \omega t)
$$

We need to:

1. Verify that it satisfies the wave equation

$$
\frac{\partial^2 y}{\partial t^2} = v^2 \frac{\partial^2 y}{\partial x^2}
$$

2. Determine the relationship between $v$, $k$, and $\omega$.

---

## Solution

We are given the function

$$
y(x,t) = A \cos(kx - \omega t)
$$

Let

$$
\phi = kx - \omega t
$$

Then

$$
y(x,t) = A \cos \phi
$$

---

### 1. Derivative with respect to time

First derivative:

$$
\frac{\partial y}{\partial t}
= -A \sin(kx - \omega t)\cdot \frac{\partial}{\partial t}(kx - \omega t)
$$

Since

$$
\frac{\partial}{\partial t}(kx - \omega t) = -\omega
$$

we get

$$
\frac{\partial y}{\partial t}
= -A \sin(kx - \omega t)(-\omega)
$$

$$
\frac{\partial y}{\partial t}
= A\omega \sin(kx - \omega t)
$$

Now take the second derivative:

$$
\frac{\partial^2 y}{\partial t^2}
= A\omega \cos(kx - \omega t)\cdot \frac{\partial}{\partial t}(kx - \omega t)
$$

$$
\frac{\partial^2 y}{\partial t^2}
= A\omega \cos(kx - \omega t)(-\omega)
$$

$$
\frac{\partial^2 y}{\partial t^2}
= -A\omega^2 \cos(kx - \omega t)
$$

So,

$$
\boxed{\frac{\partial^2 y}{\partial t^2} = -A\omega^2 \cos(kx - \omega t)}
$$

---

### 2. Derivative with respect to position

First derivative:

$$
\frac{\partial y}{\partial x}
= -A \sin(kx - \omega t)\cdot \frac{\partial}{\partial x}(kx - \omega t)
$$

Since

$$
\frac{\partial}{\partial x}(kx - \omega t) = k
$$

we get

$$
\frac{\partial y}{\partial x}
= -Ak \sin(kx - \omega t)
$$

Now take the second derivative:

$$
\frac{\partial^2 y}{\partial x^2}
= -Ak \cos(kx - \omega t)\cdot \frac{\partial}{\partial x}(kx - \omega t)
$$

$$
\frac{\partial^2 y}{\partial x^2}
= -Ak \cos(kx - \omega t)\cdot k
$$

$$
\frac{\partial^2 y}{\partial x^2}
= -Ak^2 \cos(kx - \omega t)
$$

So,

$$
\boxed{\frac{\partial^2 y}{\partial x^2} = -Ak^2 \cos(kx - \omega t)}
$$

---

### 3. Substitution into the wave equation

The wave equation is

$$
\frac{\partial^2 y}{\partial t^2} = v^2 \frac{\partial^2 y}{\partial x^2}
$$

Substitute the derivatives:

$$
-A\omega^2 \cos(kx - \omega t) = v^2(-Ak^2 \cos(kx - \omega t))
$$

Cancel the common factor $-A\cos(kx - \omega t)$:

$$
\omega^2 = v^2 k^2
$$

Taking the positive root:

$$
\omega = vk
$$

Therefore,

$$
\boxed{v = \frac{\omega}{k}}
$$

---

## Interpretation

The function

$$
y(x,t) = A\cos(kx - \omega t)
$$

is a harmonic traveling wave.

Where:

- $A$ is the amplitude
- $k$ is the wave number
- $\omega$ is the angular frequency
- $v$ is the wave speed

This function satisfies the wave equation only if

$$
\omega^2 = v^2 k^2
$$

or equivalently,

$$
\boxed{\omega = vk}
$$

and

$$
\boxed{v = \frac{\omega}{k}}
$$

---

## Final Answer

The function

$$
y(x,t) = A\cos(kx - \omega t)
$$

satisfies the wave equation

$$
\frac{\partial^2 y}{\partial t^2} = v^2 \frac{\partial^2 y}{\partial x^2}
$$

if the parameters satisfy the algebraic relation

$$
\boxed{\omega^2 = v^2 k^2}
$$

Hence,

$$
\boxed{\omega = vk}
\qquad \text{or} \qquad
\boxed{v = \frac{\omega}{k}}
$$

---

## Conclusion

By calculating the second derivative with respect to time and position, we proved that the given function is a solution of the wave equation.

The required relation between the wave speed, wave number, and angular frequency is:

$$
\boxed{v = \frac{\omega}{k}}
$$
