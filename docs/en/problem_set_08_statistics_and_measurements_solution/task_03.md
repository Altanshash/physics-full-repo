# Problem 3 – Propagation of Uncertainty

## Given

Density of a rectangular cuboid:

$$
\rho = \frac{m}{abc}
$$

Mass:

$$
m = 128.4 \pm 0.2\ \text{g}
$$

Dimensions:

$$
a = 5.20 \pm 0.02\ \text{cm}
$$

$$
b = 2.10 \pm 0.02\ \text{cm}
$$

$$
c = 1.50 \pm 0.01\ \text{cm}
$$

---

## Solution

### 1. Density

$$
\rho = \frac{m}{abc}
$$

Substitute the values:

$$
\rho = \frac{128.4}{5.20 \cdot 2.10 \cdot 1.50}
$$

$$
\rho = \frac{128.4}{16.38}
$$

$$
\rho = 7.84\ \text{g/cm}^3
$$

---

### 2. Relative Uncertainty Formula

For density:

$$
\rho = \frac{m}{abc}
$$

Using the total differential method:

$$
\frac{u(\rho)}{\rho}
=
\frac{u(m)}{m}
+
\frac{u(a)}{a}
+
\frac{u(b)}{b}
+
\frac{u(c)}{c}
$$

---

### 3. Relative Uncertainty Calculation

Mass contribution:

$$
\frac{u(m)}{m} = \frac{0.2}{128.4}
$$

$$
\frac{u(m)}{m} = 0.00156
$$

Length contribution for \(a\):

$$
\frac{u(a)}{a} = \frac{0.02}{5.20}
$$

$$
\frac{u(a)}{a} = 0.00385
$$

Length contribution for \(b\):

$$
\frac{u(b)}{b} = \frac{0.02}{2.10}
$$

$$
\frac{u(b)}{b} = 0.00952
$$

Length contribution for \(c\):

$$
\frac{u(c)}{c} = \frac{0.01}{1.50}
$$

$$
\frac{u(c)}{c} = 0.00667
$$

Total relative uncertainty:

$$
\frac{u(\rho)}{\rho}
=
0.00156 + 0.00385 + 0.00952 + 0.00667
$$

$$
\frac{u(\rho)}{\rho} = 0.02159
$$

In percent:

$$
\frac{u(\rho)}{\rho} = 2.16\%
$$

---

### 4. Absolute Uncertainty of Density

$$
u(\rho) = \rho \cdot \frac{u(\rho)}{\rho}
$$

$$
u(\rho) = 7.84 \cdot 0.02159
$$

$$
u(\rho) = 0.17\ \text{g/cm}^3
$$

---

## Final Result

$$
\rho = 7.84 \pm 0.17\ \text{g/cm}^3
$$

---

## Conclusion

The density of the rectangular cuboid is:

$$
\rho = 7.84 \pm 0.17\ \text{g/cm}^3
$$

The relative uncertainty is:

$$
\frac{u(\rho)}{\rho} = 2.16\%
$$

The largest contribution to the uncertainty comes from the measurement of \(b\), because:

$$
\frac{u(b)}{b} = 0.00952
$$

This value is greater than the other relative uncertainty contributions.
