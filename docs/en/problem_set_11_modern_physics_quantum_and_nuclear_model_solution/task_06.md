# Problem 6 – Evolution of a Wave Packet

## Given

Initial Gaussian wave packet:

$$
\psi(x,0)=e^{-\frac{x^2}{2\sigma^2}}e^{ik_0x}
$$

where:

$$
\sigma
$$

is the initial width of the packet, and:

$$
k_0
$$

is the central wave number.

Requirement:

$$
\text{Animation of } |\psi(x,t)|^2
$$

---

## Solution

### 1. Gaussian wave packet

A Gaussian wave packet is written as:

$$
\psi(x,0)=e^{-\frac{x^2}{2\sigma^2}}e^{ik_0x}
$$

The first part:

$$
e^{-\frac{x^2}{2\sigma^2}}
$$

gives the shape of the packet.

The second part:

$$
e^{ik_0x}
$$

represents the wave oscillation inside the packet.

---

### 2. Probability density

The observable quantity is the probability density:

$$
|\psi(x,t)|^2
$$

At:

$$
t = 0
$$

the packet is localized near:

$$
x = 0
$$

---

### 3. Time evolution using FFT

To simulate time evolution, the wave function is transformed from position space to momentum space using the Fourier transform:

$$
\psi(x,t) \rightarrow \phi(k,t)
$$

In momentum space, each component evolves as:

$$
\phi(k,t)=\phi(k,0)e^{-i\omega t}
$$

For a free particle:

$$
\omega = \frac{\hbar k^2}{2m}
$$

So:

$$
\phi(k,t)=\phi(k,0)e^{-i\frac{\hbar k^2}{2m}t}
$$

Then the inverse Fourier transform gives:

$$
\psi(x,t)
$$

---

### 4. Spreading of the packet

As time increases, the wave packet spreads.

This means:

$$
\Delta x
$$

increases with time.

The packet becomes wider and its maximum height decreases because the total probability remains constant.

---

### 5. Uncertainty principle interpretation

The uncertainty principle is:

$$
\Delta x \Delta p \ge \frac{\hbar}{2}
$$

A localized wave packet has a relatively small:

$$
\Delta x
$$

Therefore, it contains a range of momenta:

$$
\Delta p
$$

Different momentum components move with different speeds, causing the packet to spread.

---

## Conclusion

A Gaussian wave packet starts localized near the center.

During time evolution:

$$
|\psi(x,t)|^2
$$

spreads out.

The peak becomes lower, while the width becomes larger.

This spreading happens because the packet contains different momentum components.

It is a direct illustration of the uncertainty principle:

$$
\Delta x \Delta p \ge \frac{\hbar}{2}
$$
