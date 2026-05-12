# Problem 6 – Central Limit Theorem

## Given

Build an HTML application that simulates the distribution of the sample mean.

The application must include:

1. Choice of source distribution:
   - uniform
   - exponential
   - two-point
   - normal

2. Setting the sample size:

$$n$$

3. Setting the number of samples:

$$N$$

4. Generating sample means:

$$\bar{x}$$

5. Histogram of the distribution of sample means.

6. Comparison of the empirical standard deviation with the theoretical value:

$$\frac{\sigma}{\sqrt{n}}$$

7. Ability to overlay a Gaussian curve.

8. Brief analysis of the effect of sample size on the shape of the distribution.

---

## Solution

### 1. Central Limit Theorem Idea

The Central Limit Theorem states that if we take many random samples from a population and calculate their means, then the distribution of those sample means becomes approximately normal when the sample size is large.

This happens even if the original distribution is not normal.

---

### 2. Source Distributions

The application allows the user to choose one of four source distributions:

- Uniform distribution
- Exponential distribution
- Two-point distribution
- Normal distribution

Each distribution produces random values in a different way.

---

### 3. Sample Size and Number of Samples

The sample size is:

$$n$$

The number of generated samples is:

$$N$$

For each sample, the program generates \(n\) random values and calculates their mean.

---

### 4. Sample Mean

For one sample, the mean is calculated as:

$$\bar{x} = \frac{x_1 + x_2 + \dots + x_n}{n}$$

The program repeats this process \(N\) times and obtains \(N\) sample means:

$$\bar{x}_1,\ \bar{x}_2,\ \bar{x}_3,\ \dots,\ \bar{x}_N$$

---

### 5. Empirical Standard Deviation

The empirical standard deviation of the generated sample means is calculated from the histogram data:

$$s_{\bar{x}} = \sqrt{\frac{\sum(\bar{x}_i - \mu_{\bar{x}})^2}{N - 1}}$$

This value describes the spread of the simulated sample means.

---

### 6. Theoretical Standard Deviation

According to the Central Limit Theorem, the theoretical standard deviation of the sample mean is:

$$\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$$

where:

$$\sigma$$

is the standard deviation of the original source distribution.

---

### 7. Gaussian Curve Overlay

The application can display a Gaussian curve over the histogram.

The Gaussian curve is used to compare the simulated sample mean distribution with the normal distribution.

As the sample size increases, the histogram becomes closer to the Gaussian curve.

---

## Conclusion

The application demonstrates the Central Limit Theorem.

When the sample size \(n\) is small, the distribution of sample means may not look normal.

When the sample size \(n\) increases, the distribution of sample means becomes more bell-shaped.

The empirical standard deviation of the sample means becomes close to the theoretical value:

$$\frac{\sigma}{\sqrt{n}}$$

Therefore, increasing the sample size makes the sample mean distribution narrower and more similar to a normal distribution.
