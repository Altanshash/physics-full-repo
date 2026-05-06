# Problem 1

## Given

All resistors have the same resistance:

$$
R = 5\ \Omega
$$

Find the equivalent resistance of the circuit.

## Solution

The two resistors in the upper branch are connected in series:

$$
R_1 = 5 + 5 = 10\ \Omega
$$

In the lower branch, two resistors are connected in parallel:

$$
R_p = \frac{R \cdot R}{R + R}
$$

$$
R_p = \frac{5 \cdot 5}{5 + 5}
$$

$$
R_p = 2.5\ \Omega
$$

This parallel part is connected in series with one more resistor:

$$
R_2 = 5 + 2.5 = 7.5\ \Omega
$$

Now the upper and lower branches are connected in parallel:

$$
R_{12} = \frac{R_1 \cdot R_2}{R_1 + R_2}
$$

$$
R_{12} = \frac{10 \cdot 7.5}{10 + 7.5}
$$

$$
R_{12} = \frac{75}{17.5}
$$

$$
R_{12} \approx 4.29\ \Omega
$$

The last resistor on the right is connected in series with the whole circuit:

$$
R_{\text{eq}} = R_{12} + 5
$$

$$
R_{\text{eq}} = 4.29 + 5
$$

$$
R_{\text{eq}} \approx 9.29\ \Omega
$$

## Conclusion

The equivalent resistance of the circuit is:

$$
\boxed{R_{\text{eq}} \approx 9.29\ \Omega}
$$
