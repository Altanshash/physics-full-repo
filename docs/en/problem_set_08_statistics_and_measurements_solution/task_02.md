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

$$
R = \frac{U}{I}
$$

$$
R = \frac{5.23}{0.482}
$$

$$
R = 10.85\ \Omega
$$

---

### 2. Relative Uncertainty Formula

For the resistance:

$$
R = \frac{U}{I}
$$

Using the total differential method:

$$
dR = \frac{\partial R}{\partial U}dU + \frac{\partial R}{\partial I}dI
$$

The partial derivatives are:

$$
\frac{\partial R}{\partial U} = \frac{1}{I}
$$

$$
\frac{\partial R}{\partial I} = -\frac{U}{I^2}
$$

For maximum uncertainty:

$$
u(R) = \left|\frac{\partial R}{\partial U}\right|u(U) + \left|\frac{\partial R}{\partial I}\right|u(I)
$$

After dividing by \(R\), the relative uncertainty becomes:

$$
\frac{u(R)}{R} = \frac{u(U)}{U} + \frac{u(I)}{I}
$$

---

### 3. Relative Uncertainty Calculation

Voltage relative uncertainty:

$$
\frac{u(U)}{U} = \frac{0.04}{5.23}
$$

$$
\frac{u(U)}{U} = 0.00765
$$

Current relative uncertainty:

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
R = 10.85 \pm 0.22\ \Omega
$$

The relative uncertainty is:

$$
\frac{u(R)}{R} = 2.01\%
$$

The current measurement dominates the uncertainty because:

$$
\frac{u(I)}{I} = 0.01245
$$

is greater than:

$$
\frac{u(U)}{U} = 0.00765
$$
