# Problem 5 – Systematic vs. Statistical Errors

## Given

True value:

$$x_{\text{true}} = 10.00$$

Group A:

$$x = [10.01,\ 9.99,\ 10.02,\ 9.98,\ 10.00]$$

Group B:

$$x = [10.42,\ 10.40,\ 10.41,\ 10.43,\ 10.39]$$

Group C:

$$x = [9.6,\ 10.5,\ 10.2,\ 9.8,\ 10.4]$$

For each group, calculate:

$$\bar{x}$$

$$s$$

$$u(\bar{x}) = \frac{s}{\sqrt{n}}$$

where:

$$n = 5$$

---

## Solution

### Group A

Mean:

$$\bar{x}_A = 10.00$$

Standard deviation:

$$s_A = 0.016$$

Uncertainty of the mean:

$$u(\bar{x}_A) = \frac{0.016}{\sqrt{5}}$$

$$u(\bar{x}_A) = 0.007$$

Final result:

$$x_A = 10.00 \pm 0.007$$

Comparison with the true value:

$$\bar{x}_A - x_{\text{true}} = 10.00 - 10.00 = 0.00$$

Group A is accurate and precise.

There is no significant systematic error.

---

### Group B

Mean:

$$\bar{x}_B = 10.41$$

Standard deviation:

$$s_B = 0.016$$

Uncertainty of the mean:

$$u(\bar{x}_B) = \frac{0.016}{\sqrt{5}}$$

$$u(\bar{x}_B) = 0.007$$

Final result:

$$x_B = 10.41 \pm 0.007$$

Comparison with the true value:

$$\bar{x}_B - x_{\text{true}} = 10.41 - 10.00 = 0.41$$

Group B is precise but not accurate.

A systematic error occurs because all measurements are shifted away from the true value.

---

### Group C

Mean:

$$\bar{x}_C = 10.10$$

Standard deviation:

$$s_C = 0.387$$

Uncertainty of the mean:

$$u(\bar{x}_C) = \frac{0.387}{\sqrt{5}}$$

$$u(\bar{x}_C) = 0.173$$

Final result:

$$x_C = 10.10 \pm 0.17$$

Comparison with the true value:

$$\bar{x}_C - x_{\text{true}} = 10.10 - 10.00 = 0.10$$

Group C has large scatter.

The statistical error dominates.

---

## Summary Table

| Group | Mean | Standard Deviation | Uncertainty of Mean | Difference from True Value | Interpretation |
|---|---:|---:|---:|---:|---|
| A | 10.00 | 0.016 | 0.007 | 0.00 | Accurate and precise |
| B | 10.41 | 0.016 | 0.007 | 0.41 | Systematic error |
| C | 10.10 | 0.387 | 0.173 | 0.10 | Statistical error dominates |

---

## Possible Causes of Systematic Error

Possible causes of systematic error are:

1. Incorrect calibration of the measuring instrument.
2. Zero error of the ruler or measuring device.
3. Wrong measurement method.
4. Constant parallax error.

---

## Why More Measurements Do Not Remove Systematic Error

Increasing the number of measurements reduces statistical error.

However, systematic error does not disappear because it shifts all measurements in the same direction.

For example, if the ruler is incorrectly calibrated, every measurement will still be wrong even after many repetitions.

---

## Reflection

Compare:

$$x = 10.41 \pm 0.01$$

and:

$$x = 10.00 \pm 0.20$$

The result:

$$x = 10.41 \pm 0.01$$

is very precise, but it is not accurate because it is far from the true value.

The result:

$$x = 10.00 \pm 0.20$$

is less precise, but it is accurate because it agrees with the true value.

Therefore:

$$x = 10.00 \pm 0.20$$

is better because it contains the true value.

---

## Conclusion

Group A gives the best result because its mean value is equal to the true value and its uncertainty is small.

Group B has a systematic error because the measurements are close to each other but far from the true value.

Group C has a large statistical error because the measurements are widely scattered.

The best measurement result is not always the one with the smallest uncertainty. It must also be close to the true value.
