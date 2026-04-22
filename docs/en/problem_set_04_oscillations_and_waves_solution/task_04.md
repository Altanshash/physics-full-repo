# Problem 4 – Wave equation

## Given

The function is

$$
y(x,t)=A\cos(kx-\omega t)
$$

We need to:

1. Verify that it satisfies the wave equation
   $$
   \frac{\partial^2 y}{\partial t^2}=v^2\frac{\partial^2 y}{\partial x^2}
   $$
2. Determine the relationship between $v$, $k$, and $\omega$.

---

## Solution

### 1. Given wave function

We start with

$$
y(x,t)=A\cos(kx-\omega t)
$$

Let

$$
\phi = kx-\omega t
$$

Then the function becomes

$$
y(x,t)=A\cos\phi
$$

---

### 2. Second derivative with respect to time

First, find the first derivative with respect to $t$:

$$
\frac{\partial y}{\partial t}
=
-A\sin(kx-\omega t)\cdot \frac{\partial}{\partial t}(kx-\omega t)
$$

Since

$$
\frac{\partial}{\partial t}(kx-\omega t)=-\omega
$$

we get

$$
\frac{\partial y}{\partial t}
=
-A\sin(kx-\omega t)(-\omega)
$$

$$
\frac{\partial y}{\partial t}
=
A\omega \sin(kx-\omega t)
$$

Now take the second derivative:

$$
\frac{\partial^2 y}{\partial t^2}
=
A\omega \cos(kx-\omega t)\cdot \frac{\partial}{\partial t}(kx-\omega t)
$$

Again,

$$
\frac{\partial}{\partial t}(kx-\omega t)=-\omega
$$

so

$$
\frac{\partial^2 y}{\partial t^2}
=
A\omega \cos(kx-\omega t)(-\omega)
$$

$$
\frac{\partial^2 y}{\partial t^2}
=
-A\omega^2 \cos(kx-\omega t)
$$

Thus,

$$
\boxed{\frac{\partial^2 y}{\partial t^2}=-A\omega^2\cos(kx-\omega t)}
$$

---

### 3. Second derivative with respect to position

First, find the first derivative with respect to $x$:

$$
\frac{\partial y}{\partial x}
=
-A\sin(kx-\omega t)\cdot \frac{\partial}{\partial x}(kx-\omega t)
$$

Since

$$
\frac{\partial}{\partial x}(kx-\omega t)=k
$$

we get

$$
\frac{\partial y}{\partial x}
=
-Ak\sin(kx-\omega t)
$$

Now take the second derivative:

$$
\frac{\partial^2 y}{\partial x^2}
=
-Ak\cos(kx-\omega t)\cdot \frac{\partial}{\partial x}(kx-\omega t)
$$

So,

$$
\frac{\partial^2 y}{\partial x^2}
=
-Ak\cos(kx-\omega t)\cdot k
$$

$$
\frac{\partial^2 y}{\partial x^2}
=
-Ak^2\cos(kx-\omega t)
$$

Thus,

$$
\boxed{\frac{\partial^2 y}{\partial x^2}=-Ak^2\cos(kx-\omega t)}
$$

---

### 4. Substitute into the wave equation

The wave equation is

$$
\frac{\partial^2 y}{\partial t^2}
=
v^2\frac{\partial^2 y}{\partial x^2}
$$

Substitute the derivatives:

$$
-A\omega^2\cos(kx-\omega t)
=
v^2\left(-Ak^2\cos(kx-\omega t)\right)
$$

Cancel the common factor

$$
-A\cos(kx-\omega t)
$$

and obtain

$$
\omega^2=v^2k^2
$$

Taking the positive root for wave speed:

$$
\omega = vk
$$

Therefore,

$$
\boxed{v=\frac{\omega}{k}}
$$

---

## Interpretation

The function

$$
y(x,t)=A\cos(kx-\omega t)
$$

is a standard harmonic traveling wave.

- $A$ is the amplitude.
- $k$ is the wave number.
- $\omega$ is the angular frequency.
- $v$ is the wave speed.

After substitution into the wave equation, we get the condition

$$
\omega^2=v^2k^2
$$

This means the function is a solution of the wave equation only when the parameters satisfy

$$
\boxed{\omega = vk}
$$

or equivalently

$$
\boxed{v=\frac{\omega}{k}}
$$

So, the wave speed depends on the ratio of angular frequency to wave number.

---

## Final Answer

The function

$$
y(x,t)=A\cos(kx-\omega t)
$$

satisfies the wave equation

$$
\frac{\partial^2 y}{\partial t^2}=v^2\frac{\partial^2 y}{\partial x^2}
$$

provided that

$$
\omega^2=v^2k^2
$$

Hence, the relation between $v$, $k$, and $\omega$ is

$$
\boxed{v=\frac{\omega}{k}}
$$

---

## Conclusion

We verified by direct differentiation that the given function satisfies the wave equation.  
The required algebraic relation between the wave speed, wave number, and angular frequency is

$$
\boxed{\omega = vk}
\quad \text{or} \quad
\boxed{v=\frac{\omega}{k}}
$$
