# Problem 5 – Kepler's Third Law

## Given

We analyze data for several planets.

For each planet, we use:

- $a$ — semi-major axis
- $T$ — orbital period

According to Kepler's third law:

$$
T^2 = C a^3
$$

where $C$ is a proportionality constant.

The goal is to plot:

$$
T^2 \text{ as a function of } a^3
$$

and perform linear regression.

---

## Solution

### 1. Planetary Data

Example planetary data:

| Planet  | Semi-major axis $a$ | Period $T$ |
|---------|----------------------|------------|
| Mercury | 0.387 | 0.241 |
| Venus   | 0.723 | 0.615 |
| Earth   | 1.000 | 1.000 |
| Mars    | 1.524 | 1.881 |
| Jupiter | 5.203 | 11.862 |
| Saturn  | 9.537 | 29.457 |

Here, $a$ is measured in astronomical units and $T$ is measured in years.

---

### 2. Transforming the Data

For each planet, calculate:

$$
x = a^3
$$

and:

$$
y = T^2
$$

Then Kepler's third law becomes a linear relation:

$$
y = Cx
$$

or:

$$
T^2 = C a^3
$$

---

### 3. Linear Regression

We fit the data using a straight line:

$$
y = mx + b
$$

For Kepler's third law, the intercept should be close to zero:

$$
b \approx 0
$$

The slope of the line gives the proportionality constant:

$$
C \approx m
$$

Using planetary data in astronomical units and years, the expected value is approximately:

$$
C \approx 1
$$

---

### 4. Goodness of Fit

The quality of the linear fit is measured by the coefficient of determination:

$$
R^2
$$

If:

$$
R^2 \approx 1
$$

then the fit is very good.

This means the data strongly supports Kepler's third law.

---

## Conclusion

Kepler's third law states that the square of the orbital period is proportional to the cube of the semi-major axis:

$$
T^2 = C a^3
$$

After transforming the data into $a^3$ and $T^2$, the relationship becomes linear.

The slope of the regression line gives the proportionality constant $C$.

For planets measured in astronomical units and years:

$$
C \approx 1
$$

A value of $R^2$ close to 1 shows that the planetary data fits Kepler's third law very well.
