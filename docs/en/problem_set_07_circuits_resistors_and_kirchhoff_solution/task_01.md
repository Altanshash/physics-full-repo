# Problem 1

## Given

Find the equivalent resistance of the circuit shown in the figure.

All resistors have the same resistance:

\[
R = 5\ \Omega
\]

---

# Solution

The top branch contains two resistors connected in series:

\[
R_1 = 5 + 5 = 10\ \Omega
\]

In the bottom branch, there is first one resistor:

\[
R = 5\ \Omega
\]

Then two resistors are connected in parallel:

\[
R_p = \frac{R \cdot R}{R + R}
\]

\[
R_p = \frac{5 \times 5}{5 + 5}
\]

\[
R_p = \frac{25}{10} = 2.5\ \Omega
\]

Now calculate the total resistance of the bottom branch:

\[
R_2 = 5 + 2.5 = 7.5\ \Omega
\]

The top and bottom branches are connected in parallel:

\[
R_{12} = \frac{R_1 \cdot R_2}{R_1 + R_2}
\]

\[
R_{12} = \frac{10 \times 7.5}{10 + 7.5}
\]

\[
R_{12} = \frac{75}{17.5}
\]

\[
R_{12} = 4.29\ \Omega
\]

Finally, the last resistor on the right is connected in series:

\[
R_{\text{eq}} = R_{12} + 5
\]

\[
R_{\text{eq}} = 4.29 + 5
\]

\[
R_{\text{eq}} = 9.29\ \Omega
\]

---

# Answer

\[
\boxed{R_{\text{eq}} = 9.29\ \Omega}
\]
