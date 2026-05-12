# Problem 2 – Propagation of Uncertainty Using the Total Differential Method

## Given

Resistance is determined from Ohm's law:

$$
R = \frac{U}{I}
$$

Voltage:

$$
U = 5.23 \pm 0.04\ \text{V}
$$

Current:

$$
I = 0.482 \pm 0.006\ \text{A}
$$

---

## Solution

### 1. Resistance

Using Ohm's law:

$$
R = \frac{U}{I}
$$

Substitute the values:

$$
R = \frac{5.23}{0.482}
$$

$$
R = 10.85\ \Omega
$$

---

### 2. Relative Uncertainty Formula

The resistance is:

$$
R = \frac{U}{I}
$$

Using the total differential method:

$$
\frac{u(R)}{R} = \frac{u(U)}{U} + \frac{u(I)}{I}
$$

---

### 3. Relative Uncertainty Calculation

For voltage:

$$
\frac{u(U)}{U} = \frac{0.04}{5.23}
$$

$$
\frac{u(U)}{U} = 0.00765
$$

For current:

$$
\frac{u(I)}{I} = \frac{0.006}{0.482}
$$

$$
\frac{u(I)}{I} = 0.01245
$$

Total relative uncertainty:

$$
\frac{u(R)}{R} = 0.00765 + 0.01245
$$

$$
\frac{u(R)}{R} = 0.02010
$$

In percent:

$$
\frac{u(R)}{R} = 2.01\%
$$

---

### 4. Absolute Uncertainty of Resistance

$$
u(R) = R \cdot \frac{u(R)}{R}
$$

$$
u(R) = 10.85 \cdot 0.02010
$$

$$
u(R) = 0.22\ \Omega
$$

---

## Final Result

$$
R = 10.85 \pm 0.22\ \Omega
$$

---

## Conclusion

The resistance calculated from Ohm's law is:

$$
\boxed{R = 10.85 \pm 0.22\ \Omega}
$$

The relative uncertainty is:

$$
\boxed{\frac{u(R)}{R} = 2.01\%}
$$

The current measurement dominates the uncertainty because:

$$
\frac{u(I)}{I} = 0.01245
$$

is greater than:

$$
\frac{u(U)}{U} = 0.00765
$$
