# Problem Set 8 – Statistics and Measurements

## Problem 1 – Descriptive Statistics of a Measurement Series

## Given

The measurements of a rod’s length are given in centimeters:

$$
x = [12.10,\ 12.08,\ 12.12,\ 12.11,\ 12.09,\ 12.13,\ 12.07,\ 12.10]
$$

Number of measurements:

$$
n = 8
$$

Tasks:

1. Calculate the arithmetic mean:

$$
\bar{x}
$$

2. Calculate the sample variance and standard deviation:

$$
s^2,\quad s
$$

3. Calculate the uncertainty of the mean:

$$
u(\bar{x}) = \frac{s}{\sqrt{n}}
$$

4. Provide the result in the format:

$$
x = \bar{x} \pm u(\bar{x})
$$

5. Explain the difference between the standard deviation \(s\) and the uncertainty of the mean \(u(\bar{x})\).

6. Assuming a normal distribution, calculate the intervals:

$$
\bar{x} \pm s
$$

$$
\bar{x} \pm 2s
$$

$$
\bar{x} \pm 3s
$$

and interpret them as confidence levels: 68%, 95%, and 99%.

---

# Solution

## 1. Arithmetic Mean

The arithmetic mean is calculated using the formula:

$$
\bar{x} = \frac{\sum x_i}{n}
$$

First, find the sum of all measurements:

$$
\sum x_i = 12.10 + 12.08 + 12.12 + 12.11 + 12.09 + 12.13 + 12.07 + 12.10
$$

$$
\sum x_i = 96.80
$$

Now calculate the mean:

$$
\bar{x} = \frac{96.80}{8}
$$

$$
\bar{x} = 12.10\ \text{cm}
$$

---

## 2. Sample Variance and Standard Deviation

The sample variance is calculated by the formula:

$$
s^2 = \frac{\sum (x_i - \bar{x})^2}{n - 1}
$$

Since:

$$
\bar{x} = 12.10
$$

we calculate the squared deviations:

$$
(12.10 - 12.10)^2 = 0
$$

$$
(12.08 - 12.10)^2 = 0.0004
$$

$$
(12.12 - 12.10)^2 = 0.0004
$$

$$
(12.11 - 12.10)^2 = 0.0001
$$

$$
(12.09 - 12.10)^2 = 0.0001
$$

$$
(12.13 - 12.10)^2 = 0.0009
$$

$$
(12.07 - 12.10)^2 = 0.0009
$$

$$
(12.10 - 12.10)^2 = 0
$$

The sum of squared deviations is:

$$
\sum (x_i - \bar{x})^2 = 0.0028
$$

Now calculate the sample variance:

$$
s^2 = \frac{0.0028}{8 - 1}
$$

$$
s^2 = \frac{0.0028}{7}
$$

$$
s^2 = 0.0004\ \text{cm}^2
$$

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

## 3. Uncertainty of the Mean

The uncertainty of the mean is calculated using the formula:

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

## 4. Final Result

The result should be written in the following format:

$$
x = \bar{x} \pm u(\bar{x})
$$

Therefore:

$$
x = 12.10 \pm 0.0071
$$

Final result:

$$
\boxed{x = (12.10 \pm 0.007)\ \text{cm}}
$$

---

## 5. Difference Between Standard Deviation and Uncertainty of the Mean

The standard deviation \(s\) describes how much the individual measurements are spread around the mean value.

In this problem:

$$
s = 0.02\ \text{cm}
$$

This means that the separate measurements usually differ from the average value by about \(0.02\ \text{cm}\).

The uncertainty of the mean \(u(\bar{x})\) describes how accurately the mean value has been determined.

In this problem:

$$
u(\bar{x}) = 0.0071\ \text{cm}
$$

This value is smaller than the standard deviation because it represents the uncertainty of the average, not the spread of individual measurements.

---

# 6. Confidence Intervals

## Interval 1: 68% Confidence Level

For a normal distribution, the interval

$$
\bar{x} \pm s
$$

corresponds approximately to 68%.

Substitute the values:

$$
12.10 \pm 0.02
$$

So:

$$
12.10 - 0.02 = 12.08
$$

$$
12.10 + 0.02 = 12.12
$$

Therefore:

$$
\boxed{[12.08;\ 12.12]\ \text{cm}}
$$

This interval contains approximately 68% of the measurements.

---

## Interval 2: 95% Confidence Level

For a normal distribution, the interval

$$
\bar{x} \pm 2s
$$

corresponds approximately to 95%.

Substitute the values:

$$
12.10 \pm 2(0.02)
$$

$$
12.10 \pm 0.04
$$

So:

$$
12.10 - 0.04 = 12.06
$$

$$
12.10 + 0.04 = 12.14
$$

Therefore:

$$
\boxed{[12.06;\ 12.14]\ \text{cm}}
$$

This interval contains approximately 95% of the measurements.

---

## Interval 3: 99% Confidence Level

For a normal distribution, the interval

$$
\bar{x} \pm 3s
$$

corresponds approximately to 99%.

Substitute the values:

$$
12.10 \pm 3(0.02)
$$

$$
12.10 \pm 0.06
$$

So:

$$
12.10 - 0.06 = 12.04
$$

$$
12.10 + 0.06 = 12.16
$$

Therefore:

$$
\boxed{[12.04;\ 12.16]\ \text{cm}}
$$

This interval contains approximately 99% of the measurements.

---

# Conclusion

The arithmetic mean of the rod’s length is:

$$
\boxed{\bar{x} = 12.10\ \text{cm}}
$$

The sample variance is:

$$
\boxed{s^2 = 0.0004\ \text{cm}^2}
$$

The standard deviation is:

$$
\boxed{s = 0.02\ \text{cm}}
$$

The uncertainty of the mean is:

$$
\boxed{u(\bar{x}) = 0.0071\ \text{cm}}
$$

The final measurement result is:

$$
\boxed{x = (12.10 \pm 0.007)\ \text{cm}}
$$

The measurements are very close to each other. Therefore, the measurement series is stable, and the average value is relatively precise and reliable.
