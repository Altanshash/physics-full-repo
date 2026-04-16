# Problem 2 – Energy of a Harmonic Oscillator

## Given

A harmonic oscillator has the following parameters:

- Mass: $m = 1 \ \text{kg}$
- Spring constant: $k = 100 \ \text{N/m}$
- Initial displacement: $x(0) = 2 \ \text{m}$
- Initial velocity: $v(0) = 1 \ \text{m/s}$

## Find

1. The natural frequency of the oscillator
2. The total mechanical energy of the system
3. The displacement at which the kinetic energy is equal to $50\%$ of the total energy

---

# Solution

## 1. Natural frequency

For a harmonic oscillator, the angular natural frequency is

$$
\omega_0 = \sqrt{\frac{k}{m}}
$$

Substitute the given values:

$$
\omega_0 = \sqrt{\frac{100}{1}} = \sqrt{100} = 10 \ \text{rad/s}
$$

So, the angular natural frequency is

$$
\boxed{\omega_0 = 10 \ \text{rad/s}}
$$

If we also want the ordinary frequency in hertz, then

$$
f = \frac{\omega_0}{2\pi}
$$

$$
f = \frac{10}{2\pi} \approx 1.59 \ \text{Hz}
$$

Therefore,

$$
\boxed{f \approx 1.59 \ \text{Hz}}
$$

---

## 2. Total mechanical energy

The total mechanical energy of a harmonic oscillator is the sum of kinetic and potential energies:

$$
E = \frac{1}{2}mv^2 + \frac{1}{2}kx^2
$$

At $t=0$:

$$
E = \frac{1}{2}(1)(1^2) + \frac{1}{2}(100)(2^2)
$$

Now calculate each term:

### Kinetic energy at $t=0$

$$
K_0 = \frac{1}{2}(1)(1^2) = 0.5 \ \text{J}
$$

### Potential energy at $t=0$

$$
U_0 = \frac{1}{2}(100)(2^2)
$$

$$
U_0 = 50 \cdot 4 = 200 \ \text{J}
$$

### Total energy

$$
E = 0.5 + 200 = 200.5 \ \text{J}
$$

Thus,

$$
\boxed{E = 200.5 \ \text{J}}
$$

---

## 3. Displacement when kinetic energy is 50% of total energy

We are told that the kinetic energy is half of the total energy:

$$
K = 0.5E
$$

Since the total energy is constant,

$$
E = K + U
$$

If kinetic energy is $50\%$ of the total energy, then potential energy is also $50\%$ of the total energy:

$$
U = 0.5E
$$

The potential energy of the spring is

$$
U = \frac{1}{2}kx^2
$$

Set this equal to half of the total energy:

$$
\frac{1}{2}kx^2 = 0.5E
$$

Substitute $k=100$ and $E=200.5$:

$$
\frac{1}{2}(100)x^2 = 0.5(200.5)
$$

$$
50x^2 = 100.25
$$

$$
x^2 = \frac{100.25}{50} = 2.005
$$

$$
x = \pm \sqrt{2.005}
$$

$$
x \approx \pm 1.416 \ \text{m}
$$

Therefore, the displacement is

$$
\boxed{x \approx \pm 1.42 \ \text{m}}
$$

---

# Final Answers

### 1. Natural frequency

$$
\boxed{\omega_0 = 10 \ \text{rad/s}}
$$

and

$$
\boxed{f \approx 1.59 \ \text{Hz}}
$$

### 2. Total mechanical energy

$$
\boxed{E = 200.5 \ \text{J}}
$$

### 3. Displacement when kinetic energy is 50% of total energy

$$
\boxed{x \approx \pm 1.42 \ \text{m}}
$$

---

# Interpretation

- The oscillator has a relatively high angular frequency, $\omega_0 = 10 \ \text{rad/s}$, because the spring is quite stiff compared to the mass.
- The total mechanical energy is mostly stored in the spring initially, because the initial displacement is large.
- When the kinetic energy becomes half of the total energy, the potential energy is also half of the total energy. This happens at two symmetric positions:

$$
x \approx +1.42 \ \text{m} \quad \text{and} \quad x \approx -1.42 \ \text{m}
$$

These two values are symmetric because harmonic motion is symmetric about the equilibrium position.
