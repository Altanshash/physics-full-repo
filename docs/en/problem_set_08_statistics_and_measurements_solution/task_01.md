# Problem Set 8 – Statistics and Measurements

## Problem 1 – Descriptive statistics of a measurement series

### Given

Rod length measurements in cm:

\[
x = [12.10,\ 12.08,\ 12.12,\ 12.11,\ 12.09,\ 12.13,\ 12.07,\ 12.10]
\]

Number of measurements:

\[
n = 8
\]

---

## Solution

### 1. Arithmetic mean

\[
\bar{x} = \frac{\sum x_i}{n}
\]

\[
\bar{x} = \frac{96.80}{8} = 12.10\ \text{cm}
\]

---

### 2. Sample variance and standard deviation

Sample variance:

\[
s^2 = \frac{\sum (x_i - \bar{x})^2}{n-1}
\]

\[
s^2 = 0.0004\ \text{cm}^2
\]

Standard deviation:

\[
s = \sqrt{s^2}
\]

\[
s = 0.02\ \text{cm}
\]

---

### 3. Uncertainty of the mean

\[
u(\bar{x}) = \frac{s}{\sqrt{n}}
\]

\[
u(\bar{x}) = \frac{0.02}{\sqrt{8}}
\]

\[
u(\bar{x}) \approx 0.0071\ \text{cm}
\]

---

### 4. Final result

\[
x = \bar{x} \pm u(\bar{x})
\]

\[
x = 12.10 \pm 0.0071\ \text{cm}
\]

---

### 5. Difference between standard deviation and uncertainty of the mean

The standard deviation `s` shows how much individual measurements differ from the mean value.

The uncertainty of the mean `u(x̄)` shows how accurately the mean value is determined.

So:

\[
s = 0.02\ \text{cm}
\]

\[
u(\bar{x}) = 0.0071\ \text{cm}
\]

The uncertainty of the mean is smaller because it depends on the number of measurements.

---

### 6. Normal distribution intervals

#### Interval \(\bar{x} \pm s\)

\[
12.10 \pm 0.02
\]

\[
[12.08,\ 12.12]\ \text{cm}
\]

This interval corresponds approximately to 68% confidence level.

---

#### Interval \(\bar{x} \pm 2s\)

\[
12.10 \pm 0.04
\]

\[
[12.06,\ 12.14]\ \text{cm}
\]

This interval corresponds approximately to 95% confidence level.

---

#### Interval \(\bar{x} \pm 3s\)

\[
12.10 \pm 0.06
\]

\[
[12.04,\ 12.16]\ \text{cm}
\]

This interval corresponds approximately to 99% confidence level.

---

## Conclusion

The average length of the rod is:

\[
\boxed{x = 12.10 \pm 0.0071\ \text{cm}}
\]

The sample standard deviation is:

\[
s = 0.02\ \text{cm}
\]

The measurements are close to each other, so the result is reliable. According to the normal distribution rule, most measurements should lie within the intervals \(\bar{x} \pm s\), \(\bar{x} \pm 2s\), and \(\bar{x} \pm 3s\).
