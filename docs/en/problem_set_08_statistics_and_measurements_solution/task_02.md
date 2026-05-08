# Problem 2 – Propagation of Uncertainty Using the Total Differential Method

## Given

Resistance is determined from Ohm’s law:

$$
R = \frac{U}{I}
$$

Data:

$$
U = 5.23 \pm 0.04\ \text{V}
$$

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
R \approx 10.85\ \Omega
$$

---

### 2. Relative Uncertainty Formula

For

$$
R = \frac{U}{I}
$$

the relative uncertainty is:

$$
\frac{u(R)}{R} =
\sqrt{
\left(\frac{u(U)}{U}\right)^2 +
\left(\frac{u(I)}{I}\right)^2
}
$$

---

### 3. Calculate Relative Uncertainties

For voltage:

$$
\frac{u(U)}{U} = \frac{0.04}{5.23}
$$

$$
\frac{u(U)}{U} \approx 0.00765
$$

For current:

$$
\frac{u(I)}{I} = \frac{0.006}{0.482}
$$

$$
\frac{u(I)}{I} \approx 0.01245
$$

Total relative uncertainty:

$$
\frac{u(R)}{R} =
\sqrt{(0.00765)^2 + (0.01245)^2}
$$

$$
\frac{u(R)}{R} \approx 0.01461
$$

In percent:

$$
\frac{u(R)}{R} \approx 1.46\%
$$

---

### 4. Absolute Uncertainty of Resistance

$$
u(R) = R \cdot \frac{u(R)}{R}
$$

$$
u(R) = 10.85 \cdot 0.01461
$$

$$
u(R) \approx 0.16\ \Omega
$$

---

## Final Result

$$
\boxed{R = (10.85 \pm 0.16)\ \Omega}
$$

---

## Which Measurement Dominates the Uncertainty?

Voltage relative uncertainty:

$$
\frac{u(U)}{U} \approx 0.00765 = 0.765\%
$$

Current relative uncertainty:

$$
\frac{u(I)}{I} \approx 0.01245 = 1.245\%
$$

Since

$$
1.245\% > 0.765\%
$$

the current measurement \(I\) dominates the uncertainty.

---

## Conclusion

The resistance calculated from Ohm’s law is:

$$
\boxed{R = (10.85 \pm 0.16)\ \Omega}
$$

The relative uncertainty of the resistance is:

$$
\boxed{\frac{u(R)}{R} \approx 1.46\%}
$$

The current measurement contributes more to the total uncertainty than the voltage measurement.
