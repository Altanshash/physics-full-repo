# Problem Set 8 – Statistics and Measurements

## Given

Measurement series of a rod’s length (in cm):

\[
x = [12.10,\ 12.08,\ 12.12,\ 12.11,\ 12.09,\ 12.13,\ 12.07,\ 12.10]
\]

Number of measurements:

\[
n = 8
\]

---

## Solution

### 1. Arithmetic Mean

\[
\bar{x} = \frac{\sum x_i}{n}
\]

\[
\bar{x} = \frac{96.80}{8} = 12.10 \text{ cm}
\]

---

### 2. Sample Variance and Standard Deviation

Sample variance:

\[
s^2 = \frac{\sum (x_i - \bar{x})^2}{n-1}
\]

\[
s^2 = 0.0004 \text{ cm}^2
\]

Standard deviation:

\[
s = \sqrt{s^2}
\]

\[
s = \sqrt{0.0004} = 0.02 \text{ cm}
\]

---

### 3. Uncertainty of the Mean

\[
u(\bar{x}) = \frac{s}{\sqrt{n}}
\]

\[
u(\bar{x}) = \frac{0.02}{\sqrt{8}} \approx 0.0071 \text{ cm}
\]

---

### 4. Final Result

\[
x = \bar{x} \pm u(\bar{x})
\]

\[
x = (12.10 \pm 0.007) \text{ cm}
\]

---

## Difference Between Standard Deviation and Uncertainty of the Mean

The standard deviation \(s\) describes how much the individual measurements are spread around the mean value.

The uncertainty of the mean \(u(\bar{x})\) describes how accurately the mean value has been determined.

Thus:

\[
s = 0.02 \text{ cm}
\]

represents the spread of measurements, while

\[
u(\bar{x}) = 0.0071 \text{ cm}
\]

represents the precision of the average value.

---

## 5. Confidence Intervals

### \(\bar{x} \pm s\)

\[
12.10 \pm 0.02
\]

\[
[12.08;\ 12.12] \text{ cm}
\]

This interval contains approximately 68% of the measurements.

---

### \(\bar{x} \pm 2s\)

\[
12.10 \pm 0.04
\]

\[
[12.06;\ 12.14] \text{ cm}
\]

This interval contains approximately 95% of the measurements.

---

### \(\bar{x} \pm 3s\)

\[
12.10 \pm 0.06
\]

\[
[12.04;\ 12.16] \text{ cm}
\]

This interval contains approximately 99% of the measurements.

---

# Conclusion

According to the given measurements, the average length of the rod is:

\[
\boxed{x = (12.10 \pm 0.007) \text{ cm}}
\]

Standard deviation:

\[
\boxed{s = 0.02 \text{ cm}}
\]

Uncertainty of the mean:

\[
\boxed{u(\bar{x}) = 0.0071 \text{ cm}}
\]

The measurements are close to each other, indicating that the result is relatively precise and reliable.
