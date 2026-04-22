# Problem 3 – Harmonic wave

## Given

The wave equation is

$$
y(x,t)=A\sin(kx-\omega t)
$$

We need to:

1. Determine the wavelength.
2. Determine the phase velocity.
3. Calculate $v$ for $k=4\pi$, $\omega=20\pi$.
4. Check whether the point $x=\lambda$ oscillates in phase with the point $x=0$.

---

## Solution

### 1. Wavelength

For a harmonic wave

$$
y(x,t)=A\sin(kx-\omega t),
$$

the wave number $k$ is related to the wavelength $\lambda$ by

$$
k=\frac{2\pi}{\lambda}.
$$

Solve for $\lambda$:

$$
\lambda=\frac{2\pi}{k}.
$$

So, the wavelength is

$$
\boxed{\lambda=\frac{2\pi}{k}}.
$$

---

### 2. Phase velocity

A point of constant phase satisfies

$$
kx-\omega t=\text{constant}.
$$

Differentiate with respect to time:

$$
\frac{d}{dt}(kx-\omega t)=0.
$$

This gives

$$
k\frac{dx}{dt}-\omega=0.
$$

Hence,

$$
\frac{dx}{dt}=\frac{\omega}{k}.
$$

The phase velocity is therefore

$$
\boxed{v=\frac{\omega}{k}}.
$$

---

### 3. Calculate $v$ for $k=4\pi$, $\omega=20\pi$

Use the formula

$$
v=\frac{\omega}{k}.
$$

Substitute the given values:

$$
v=\frac{20\pi}{4\pi}.
$$

Simplify:

$$
v=5.
$$

So, the phase velocity is

$$
\boxed{v=5}.
$$

If SI units are assumed, then

$$
\boxed{v=5\ \text{m/s}}.
$$

---

### 4. Does the point $x=\lambda$ oscillate in phase with the point $x=0$?

At $x=0$:

$$
y(0,t)=A\sin(0-\omega t)=A\sin(-\omega t).
$$

At $x=\lambda$:

$$
y(\lambda,t)=A\sin(k\lambda-\omega t).
$$

Since

$$
\lambda=\frac{2\pi}{k},
$$

we have

$$
k\lambda=k\cdot \frac{2\pi}{k}=2\pi.
$$

Therefore,

$$
y(\lambda,t)=A\sin(2\pi-\omega t).
$$

Because the sine function is periodic with period $2\pi$,

$$
\sin(2\pi-\omega t)=\sin(-\omega t).
$$

So,

$$
y(\lambda,t)=y(0,t).
$$

This means the points $x=\lambda$ and $x=0$ have the same displacement at every moment of time, so they oscillate **in phase**.

Thus, the answer is

$$
\boxed{\text{Yes, }x=\lambda\text{ and }x=0\text{ oscillate in phase.}}
$$

---

## Interpretation

- The wavelength is the distance between two nearest points that oscillate in the same phase.
- The phase velocity shows how fast a point of constant phase moves along the wave.
- If two points are separated by one full wavelength, their phase difference is

$$
\Delta \varphi = k\lambda = 2\pi,
$$

which means they are in the same phase.

---

## Final Answers

$$
\boxed{\lambda=\frac{2\pi}{k}}
$$

$$
\boxed{v=\frac{\omega}{k}}
$$

For $k=4\pi$ and $\omega=20\pi$:

$$
\boxed{v=5}
$$

And:

$$
\boxed{x=\lambda \text{ oscillates in phase with } x=0}
$$
