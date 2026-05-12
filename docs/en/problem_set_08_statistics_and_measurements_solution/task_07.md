# Problem 7 – Simple Pendulum: Measurement of g

## Given

We need to build an HTML application to measure the acceleration due to gravity using a simple pendulum.

The formula for gravitational acceleration is:

$$g = 4\pi^2\frac{L}{T^2}$$

where:

$$L$$

is the pendulum length,

$$T$$

is the oscillation period,

$$g$$

is the acceleration due to gravity.

The user sets:

$$L$$

and its uncertainty:

$$u(L)$$

The period is determined from recorded times:

$$T_i = t_{i+1} - t_i$$

The mean period is:

$$\bar{T}$$

The standard deviation of periods is:

$$s_T$$

The uncertainty of the mean period is:

$$u(T) = \frac{s_T}{\sqrt{n}}$$

---

## Solution

### 1. Recording the Motion

The first press of the spacebar starts the pendulum motion and the stopwatch.

Each next press of the spacebar records the time when the pendulum passes through the minimum position.

The recorded times are:

$$t_1,\ t_2,\ t_3,\ \dots,\ t_n$$

---

### 2. Period Calculation

The periods are calculated from successive recorded times:

$$T_i = t_{i+1} - t_i$$

For example:

$$T_1 = t_2 - t_1$$

$$T_2 = t_3 - t_2$$

$$T_3 = t_4 - t_3$$

---

### 3. Mean Period

The mean period is calculated as:

$$\bar{T} = \frac{T_1 + T_2 + \dots + T_n}{n}$$

---

### 4. Standard Deviation of Periods

The standard deviation is:

$$s_T = \sqrt{\frac{\sum (T_i - \bar{T})^2}{n - 1}}$$

---

### 5. Uncertainty of the Mean Period

The uncertainty of the mean period is:

$$u(T) = \frac{s_T}{\sqrt{n}}$$

---

### 6. Calculation of g

Using the pendulum formula:

$$g = 4\pi^2\frac{L}{\bar{T}^2}$$

---

### 7. Uncertainty Propagation

The uncertainty of g is calculated by:

$$u(g) = \sqrt{\left(\frac{\partial g}{\partial L}u(L)\right)^2 + \left(\frac{\partial g}{\partial T}u(T)\right)^2}$$

The partial derivatives are:

$$\frac{\partial g}{\partial L} = \frac{4\pi^2}{T^2}$$

$$\frac{\partial g}{\partial T} = -\frac{8\pi^2L}{T^3}$$

Therefore:

$$u(g) = \sqrt{\left(\frac{4\pi^2}{T^2}u(L)\right)^2 + \left(\frac{8\pi^2L}{T^3}u(T)\right)^2}$$

---

### 8. Final Result

The result is displayed as:

$$g = \hat{g} \pm u(g)$$

The application also shows the percentage contribution of uncertainty from:

$$L$$

and:

$$T$$

---

## Conclusion

The application allows the user to measure the acceleration due to gravity using a simple pendulum.

The period is obtained from repeated spacebar presses, and at least 5 periods should be recorded.

The mean period and its uncertainty are calculated from the measured periods.

Then the value of gravitational acceleration is determined by:

$$g = 4\pi^2\frac{L}{\bar{T}^2}$$

The uncertainty of the final result depends on both the uncertainty of the pendulum length and the uncertainty of the measured period.

The final result is written as:

$$g = \hat{g} \pm u(g)$$
