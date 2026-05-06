# Problem 7

## Given

$$
R_1 = 6\ \Omega
$$

$$
R_2 = 4\ \Omega
$$

$$
R_3 = 3\ \Omega
$$

$$
R_4 = 12\ \Omega
$$

$$
U = 3\ V
$$

Find:

- Equivalent resistance
- Potential difference between points \(A\) and \(B\)

---

# Solution

Top branch:

$$
R_{\text{top}} = R_1 + R_2
$$

$$
R_{\text{top}} = 6 + 4 = 10\ \Omega
$$

Bottom branch:

$$
R_{\text{bottom}} = R_3 + R_4
$$

$$
R_{\text{bottom}} = 3 + 12 = 15\ \Omega
$$

The two branches are connected in parallel:

$$
R_{\text{eq}} = \frac{R_{\text{top}} \cdot R_{\text{bottom}}}{R_{\text{top}} + R_{\text{bottom}}}
$$

$$
R_{\text{eq}} = \frac{10 \cdot 15}{10 + 15}
$$

$$
R_{\text{eq}} = \frac{150}{25}
$$

$$
R_{\text{eq}} = 6\ \Omega
$$

Current in the top branch:

$$
I_{\text{top}} = \frac{3}{10} = 0.3\ A
$$

Current in the bottom branch:

$$
I_{\text{bottom}} = \frac{3}{15} = 0.2\ A
$$

Voltage drop across \(R_1\):

$$
U_1 = I_{\text{top}} \cdot R_1
$$

$$
U_1 = 0.3 \cdot 6 = 1.8\ V
$$

Voltage drop across \(R_3\):

$$
U_3 = I_{\text{bottom}} \cdot R_3
$$

$$
U_3 = 0.2 \cdot 3 = 0.6\ V
$$

Potential difference between points \(A\) and \(B\):

$$
U_{AB} = U_1 - U_3
$$

$$
U_{AB} = 1.8 - 0.6
$$

$$
U_{AB} = 1.2\ V
$$

---

# Conclusion

Equivalent resistance:

$$
\boxed{R_{\text{eq}} = 6\ \Omega}
$$

Potential difference between points \(A\) and \(B\):

$$
\boxed{U_{AB} = 1.2\ V}
$$
