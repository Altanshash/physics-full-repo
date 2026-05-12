# Problem Set 8 – Statistics and Measurements

## Problem 1 – Descriptive Statistics of a Measurement Series

## Given

The measurements of a rod's length are given in centimeters:

$$
x = [12.10,\ 12.08,\ 12.12,\ 12.11,\ 12.09,\ 12.13,\ 12.07,\ 12.10]
$$

The number of measurements is:

$$
n = 8
$$

---

## Solution

### 1. Arithmetic Mean

The arithmetic mean is calculated by the formula:

$$
\bar{x} = \frac{\sum x_i}{n}
$$

Substitute the values:

$$
\bar{x} =
\frac{12.10 + 12.08 + 12.12 + 12.11 + 12.09 + 12.13 + 12.07 + 12.10}{8}
$$

$$
\bar{x} = \frac{96.80}{8}
$$

$$
\bar{x} = 12.10\ \text{cm}
$$

---

### 2. Sample Variance

The sample variance is calculated by the formula:

$$
s^2 = \frac{\sum (x_i - \bar{x})^2}{n - 1}
$$

Calculation:

$$
s^2 = \frac{0.0028}{7}
$$

$$
s^2 = 0.0004\ \text{cm}^2
$$

---

### 3. Standard Deviation

The standard deviation is:

$$
s = \sqrt{s^2}
$$

$$
s = \sqrt{0.0004}
$$

$$
s = 0.02\ \text{cm}
$$

---

### 4. Uncertainty of the Mean

The uncertainty of the mean is calculated by the formula:

$$
u(\bar{x}) = \frac{s}{\sqrt{n}}
$$

Substitute the values:

$$
u(\bar{x}) = \frac{0.02}{\sqrt{8}}
$$

$$
u(\bar{x}) \approx 0.0071\ \text{cm}
$$

---

## Final Result

The result is written in the form:

$$
x = \bar{x} \pm u(\bar{x})
$$

Therefore:

$$
x = 12.10 \pm 0.0071\ \text{cm}
$$

Rounded result:

$$
\boxed{x = 12.10 \pm 0.01\ \text{cm}}
$$

---

## Difference Between Standard Deviation and Uncertainty of the Mean

The standard deviation shows how much individual measurements differ from the mean value.

The uncertainty of the mean shows how accurately the mean value is determined.

In this problem:

$$
s = 0.02\ \text{cm}
$$

$$
u(\bar{x}) = 0.0071\ \text{cm}
$$

The uncertainty of the mean is smaller than the standard deviation because it depends on the number of measurements.

---

## Normal Distribution Intervals

### Interval 1

For one standard deviation:

$$
\bar{x} \pm s
$$

$$
12.10 \pm 0.02
$$

$$
[12.08,\ 12.12]\ \text{cm}
$$

This interval corresponds approximately to a 68% confidence level.

---

### Interval 2

For two standard deviations:

$$
\bar{x} \pm 2s
$$

$$
12.10 \pm 2(0.02)
$$

$$
12.10 \pm 0.04
$$

$$
[12.06,\ 12.14]\ \text{cm}
$$

This interval corresponds approximately to a 95% confidence level.

---

### Interval 3

For three standard deviations:

$$
\bar{x} \pm 3s
$$

$$
12.10 \pm 3(0.02)
$$

$$
12.10 \pm 0.06
$$

$$
[12.04,\ 12.16]\ \text{cm}
$$

This interval corresponds approximately to a 99% confidence level.

---

## Conclusion

The average length of the rod is:

$$
\boxed{x = 12.10 \pm 0.01\ \text{cm}}
$$

The sample variance is:

$$
s^2 = 0.0004\ \text{cm}^2
$$

The standard deviation is:

$$
s = 0.02\ \text{cm}
$$

The measurements are close to each other. Therefore, the measurement series is consistent, and the final result is reliable.
