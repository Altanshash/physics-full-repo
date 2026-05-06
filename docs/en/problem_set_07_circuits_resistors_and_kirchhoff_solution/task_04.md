# Problem 4

## Given

$$
R_1 = 20\ \Omega
$$

$$
R_2 = 60\ \Omega
$$

$$
R_3 = 30\ \Omega
$$

$$
R_4 = 10\ \Omega
$$

$$
U = 200\ V
$$

Find:

- Voltage across resistor \(R_3\)
- Current through resistor \(R_3\)

---

# Solution

Resistors \(R_2\) and \(R_3\) are connected in parallel.

Equivalent resistance:

$$
R_{23} = \frac{R_2 \cdot R_3}{R_2 + R_3}
$$

$$
R_{23} = \frac{60 \times 30}{60 + 30}
$$

$$
R_{23} = \frac{1800}{90}
$$

$$
R_{23} = 20\ \Omega
$$

Now calculate total resistance:

$$
R_{\text{eq}} = R_1 + R_{23} + R_4
$$

$$
R_{\text{eq}} = 20 + 20 + 10
$$

$$
R_{\text{eq}} = 50\ \Omega
$$

Total current in the circuit:

$$
I = \frac{U}{R_{\text{eq}}}
$$

$$
I = \frac{200}{50}
$$

$$
I = 4\ A
$$

Voltage across the parallel branch:

$$
U_{23} = I \cdot R_{23}
$$

$$
U_{23} = 4 \times 20
$$

$$
U_{23} = 80\ V
$$

Since \(R_2\) and \(R_3\) are parallel:

$$
U_3 = U_{23}
$$

$$
U_3 = 80\ V
$$

Current through resistor \(R_3\):

$$
I_3 = \frac{U_3}{R_3}
$$

$$
I_3 = \frac{80}{30}
$$

$$
I_3 \approx 2.67\ A
$$

---

# Conclusion

Voltage across resistor \(R_3\):

$$
\boxed{U_3 = 80\ V}
$$

Current through resistor \(R_3\):

$$
\boxed{I_3 \approx 2.67\ A}
$$
