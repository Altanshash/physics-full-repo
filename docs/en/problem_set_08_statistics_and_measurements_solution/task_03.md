# Problem 3 – Propagation of Uncertainty

## Given

The density of a rectangular cuboid is determined by the formula:

$$
\rho = \frac{m}{abc}
$$

where:

$$
\rho
$$

is the density,

$$
m
$$

is the mass of the cuboid,

$$
a,\ b,\ c
$$

are the dimensions of the cuboid.

The measured values are:

$$
m = 128.4 \pm 0.2\ \text{g}
$$

$$
a = 5.20 \pm 0.02\ \text{cm}
$$

$$
b = 2.10 \pm 0.02\ \text{cm}
$$

$$
c = 1.50 \pm 0.01\ \text{cm}
$$

Therefore:

$$
u(m) = 0.2\ \text{g}
$$

$$
u(a) = 0.02\ \text{cm}
$$

$$
u(b) = 0.02\ \text{cm}
$$

$$
u(c) = 0.01\ \text{cm}
$$

---

## Solution

### 1. Calculation of Density

The density is calculated as:

$$
\rho = \frac{m}{abc}
$$

Substitute the measured values:

$$
\rho = \frac{128.4}{5.20 \cdot 2.10 \cdot 1.50}
$$

First calculate the volume:

$$
V = abc
$$

$$
V = 5.20 \cdot 2.10 \cdot 1.50
$$

$$
V = 16.38\ \text{cm}^3
$$

Now calculate the density:

$$
\rho = \frac{128.4}{16.38}
$$

$$
\rho = 7.84\ \text{g/cm}^3
$$

---

### 2. Total Differential Method

The formula for density is:

$$
\rho = \frac{m}{abc}
$$

Using the total differential method:

$$
d\rho =
\frac{\partial \rho}{\partial m}dm
+
\frac{\partial \rho}{\partial a}da
+
\frac{\partial \rho}{\partial b}db
+
\frac{\partial \rho}{\partial c}dc
$$

The partial derivatives are:

$$
\frac{\partial \rho}{\partial m} = \frac{1}{abc}
$$

$$
\frac{\partial \rho}{\partial a} = -\frac{m}{a^2bc}
$$

$$
\frac{\partial \rho}{\partial b} = -\frac{m}{ab^2c}
$$

$$
\frac{\partial \rho}{\partial c} = -\frac{m}{abc^2}
$$

For maximum uncertainty, absolute values are used:

$$
u(\rho) =
\left|\frac{\partial \rho}{\partial m}\right|u(m)
+
\left|\frac{\partial \rho}{\partial a}\right|u(a)
+
\left|\frac{\partial \rho}{\partial b}\right|u(b)
+
\left|\frac{\partial \rho}{\partial c}\right|u(c)
$$

After dividing by the density, the relative uncertainty formula becomes:

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

For mass:

$$
\frac{u(m)}{m} = \frac{0.2}{128.4}
$$

$$
\frac{u(m)}{m} = 0.00156
$$

For dimension a:

$$
\frac{u(a)}{a} = \frac{0.02}{5.20}
$$

$$
\frac{u(a)}{a} = 0.00385
$$

For dimension b:

$$
\frac{u(b)}{b} = \frac{0.02}{2.10}
$$

$$
\frac{u(b)}{b} = 0.00952
$$

For dimension c:

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
\frac{u(\rho)}{\rho} = 0.02160
$$

In percent:

$$
\frac{u(\rho)}{\rho} = 2.16\%
$$

---

### 4. Absolute Uncertainty of Density

The absolute uncertainty is:

$$
u(\rho) = \rho \cdot \frac{u(\rho)}{\rho}
$$

Substitute the values:

$$
u(\rho) = 7.84 \cdot 0.02160
$$

$$
u(\rho) = 0.17\ \text{g/cm}^3
$$

---

## Final Result

The density with uncertainty is:

$$
\rho = 7.84 \pm 0.17\ \text{g/cm}^3
$$

---

## Largest Contribution to the Uncertainty

The relative uncertainty contributions are:

$$
\frac{u(m)}{m} = 0.00156
$$

$$
\frac{u(a)}{a} = 0.00385
$$

$$
\frac{u(b)}{b} = 0.00952
$$

$$
\frac{u(c)}{c} = 0.00667
$$

The largest contribution is from dimension b:

$$
\frac{u(b)}{b} = 0.00952
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

The largest contribution to the uncertainty comes from the measurement of dimension b, because its relative uncertainty is the greatest.

Therefore, the accuracy of the density measurement mainly depends on the accuracy of measuring dimension b.
