# Problem 3

## Given

All resistors have the same resistance:

$$
R = 10\ \Omega
$$

Find the equivalent resistance of the circuit.

## Solution

The left upper path has two resistors in series:

$$
R_1 = 10 + 10 = 20\ \Omega
$$

The middle path has three resistors in series:

$$
R_2 = 10 + 10 + 10 = 30\ \Omega
$$

These two paths are connected in parallel:

$$
R_{12} = \frac{R_1 \cdot R_2}{R_1 + R_2}
$$

$$
R_{12} = \frac{20 \cdot 30}{20 + 30}
$$

$$
R_{12} = \frac{600}{50} = 12\ \Omega
$$

The right side has two resistors in series:

$$
R_3 = 10 + 10 = 20\ \Omega
$$

Now add them in series:

$$
R_4 = R_{12} + R_3
$$

$$
R_4 = 12 + 20 = 32\ \Omega
$$

The bottom resistor is connected in parallel with this part:

$$
R_{\text{eq}} = \frac{32 \cdot 10}{32 + 10}
$$

$$
R_{\text{eq}} = \frac{320}{42}
$$

$$
R_{\text{eq}} \approx 7.62\ \Omega
$$

## Conclusion

$$
\boxed{R_{\text{eq}} \approx 7.62\ \Omega}
$$
