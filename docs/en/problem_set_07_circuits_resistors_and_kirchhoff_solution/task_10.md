# Problem 10

## Given

$$
R_1 = 20\ \Omega
$$

$$
R_2 = 10\ \Omega
$$

$$
r_1 = 1\ \Omega
$$

$$
r_2 = 1\ \Omega
$$

$$
\mathcal{E}_1 = 4.5\ V
$$

$$
\mathcal{E}_2 = 9\ V
$$

Find the current through the ammeter.

---

# Solution

The right branch contains:

- resistor \(R_2 = 10\ \Omega\)
- internal resistance \(r_2 = 1\ \Omega\)

connected in series:

$$
R_{right} = 10 + 1
$$

$$
R_{right} = 11\ \Omega
$$

Now total resistance of the circuit:

$$
R_{eq} = R_1 + r_1 + R_{right}
$$

$$
R_{eq} = 20 + 1 + 11
$$

$$
R_{eq} = 32\ \Omega
$$

The sources oppose each other:

$$
\mathcal{E}_{eq} = \mathcal{E}_2 - \mathcal{E}_1
$$

$$
\mathcal{E}_{eq} = 9 - 4.5
$$

$$
\mathcal{E}_{eq} = 4.5\ V
$$

Using Ohm’s law:

$$
I = \frac{\mathcal{E}_{eq}}{R_{eq}}
$$

$$
I = \frac{4.5}{32}
$$

$$
I = 0.1406\ A
$$

---

# Conclusion

The current through the ammeter is:

$$
\boxed{I_A \approx 0.141\ A}
$$

or

$$
\boxed{I_A \approx 141\ mA}
$$
