# Problem Set 8 – Statistics and Measurements

## Given

Measurements of a rod’s length in cm:

$$
x = [12.10,\ 12.08,\ 12.12,\ 12.11,\ 12.09,\ 12.13,\ 12.07,\ 12.10]
$$

$$
n = 8
$$

---

## Solution

### 1. Arithmetic Mean

$$
\bar{x} = \frac{\sum x_i}{n}
$$

$$
\bar{x} = \frac{96.80}{8} = 12.10\ \text{cm}
$$

---

### 2. Sample Variance and Standard Deviation

Sample variance:

$$
s^2 = \frac{\sum (x_i - \bar{x})^2}{n - 1}
$$

$$
s^2 = 0.0004\ \text{cm}^2
$$

Standard deviation:

$$
s = \sqrt{s^2}
$$

$$
s = \sqrt{0.0004} = 0.02\ \text{cm}
$$

---

### 3. Uncertainty of the Mean

$$
u(\bar{x}) = \frac{s}{\sqrt{n}}
$$

$$
u(\bar{x}) = \frac{0.02}{\sqrt{8}} \approx 0.0071\ \text{cm}
$$

---

### 4. Final Result

$$
x = \bar{x} \pm u(\bar{x})
$$

$$
x = (12.10 \pm 0.007)\ \text{cm}
$$

---

## Difference Between Standard Deviation and Uncertainty of the Mean

The standard deviation \(s\) shows how much the individual measurements are spread around the mean value.

The uncertainty of the mean \(u(\bar{x})\) shows how accurately the mean value is determined.

---

## Confidence Intervals

### 1σ interval

$$
\bar{x} \pm s = 12.10 \pm 0.02
$$

$$
[12.08;\ 12.12]\ \text{cm}
$$

This interval corresponds to approximately 68%.

### 2σ interval

$$
\bar{x} \pm 2s = 12.10 \pm 0.04
$$

$$
[12.06;\ 12.14]\ \text{cm}
$$

This interval corresponds to approximately 95%.

### 3σ interval

$$
\bar{x} \pm 3s = 12.10 \pm 0.06
$$

$$
[12.04;\ 12.16]\ \text{cm}
$$

This interval corresponds to approximately 99%.

---

## Conclusion

The average length of the rod is:

$$
\boxed{x = (12.10 \pm 0.007)\ \text{cm}}
$$

The standard deviation is:

$$
\boxed{s = 0.02\ \text{cm}}
$$

The uncertainty of the mean is:

$$
\boxed{u(\bar{x}) = 0.0071\ \text{cm}}
$$

The measurements are close to each other, so the result is relatively precise and reliable.
