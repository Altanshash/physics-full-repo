# Problem Set 8 – Statistics and Measurements

## Problem 1 – Descriptive Statistics of a Measurement Series

## Given

Measurements of a rod’s length (in cm):

$$
x = [12.10,\ 12.08,\ 12.12,\ 12.11,\ 12.09,\ 12.13,\ 12.07,\ 12.10]
$$

Number of measurements:

$$
n = 8
$$

---

# Solution

## 1. Arithmetic Mean

The arithmetic mean is calculated using:

$$
\bar{x} = \frac{\sum x_i}{n}
$$

Substituting the values:

$$
\bar{x} =
\frac{
12.10 + 12.08 + 12.12 + 12.11 + 12.09 + 12.13 + 12.07 + 12.10
}{8}
$$

$$
\bar{x} = \frac{96.80}{8}
$$

$$
\boxed{\bar{x} = 12.10\ \text{cm}}
$$

---

## 2. Sample Variance

The sample variance formula:

$$
s^2 = \frac{\sum (x_i - \bar{x})^2}{n-1}
$$

Calculation:

$$
s^2 = \frac{0.0028}{7}
$$

$$
\boxed{s^2 = 0.0004\ \text{cm}^2}
$$

---

## 3. Standard Deviation

The standard deviation is:

$$
s = \sqrt{s^2}
$$

$$
s = \sqrt{0.0004}
$$

$$
\boxed{s = 0.02\ \text{cm}}
$$

---

## 4. Uncertainty of the Mean

The uncertainty of the mean is calculated by:

$$
u(\bar{x}) = \frac{s}{\sqrt{n}}
$$

Substitute the known values:

$$
u(\bar{x}) = \frac{0.02}{\sqrt{8}}
$$

$$
u(\bar{x}) \approx 0.0071\ \text{cm}
$$

$$
\boxed{u(\bar{x}) \approx 0.0071\ \text{cm}}
$$

---

# Final Result

The final result is written as:

$$
x = \bar{x} \pm u(\bar{x})
$$

$$
x = 12.10 \pm 0.0071\ \text{cm}
$$

Rounded result:

$$
\boxed{x = 12.10 \pm 0.01\ \text{cm}}
$$

---

# Difference Between \(s\) and \(u(\bar{x})\)

- The standard deviation \(s\) describes how far individual measurements are spread from the mean value.
- The uncertainty of the mean \(u(\bar{x})\) describes how accurately the mean value is determined.

Values obtained:

$$
s = 0.02\ \text{cm}
$$

$$
u(\bar{x}) = 0.0071\ \text{cm}
$$

---

# Normal Distribution Intervals

## Interval \( \bar{x} \pm s \)

$$
12.10 \pm 0.02
$$

$$
[12.08,\ 12.12]\ \text{cm}
$$

This interval corresponds approximately to a **68% confidence level**.

---

## Interval \( \bar{x} \pm 2s \)

$$
12.10 \pm 0.04
$$

$$
[12.06,\ 12.14]\ \text{cm}
$$

This interval corresponds approximately to a **95% confidence level**.

---

## Interval \( \bar{x} \pm 3s \)

$$
12.10 \pm 0.06
$$

$$
[12.04,\ 12.16]\ \text{cm}
$$

This interval corresponds approximately to a **99% confidence level**.

---

# Conclusion

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

The measurements are close to each other, which indicates good measurement consistency and reliability.
