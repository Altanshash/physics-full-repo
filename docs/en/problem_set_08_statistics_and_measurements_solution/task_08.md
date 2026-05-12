# Problem 8 – Mass-Spring Oscillator

## Given

We need to build an HTML application to determine the spring constant by measuring the period of oscillations of a mass-spring system.

The formula for the spring constant is:

$$k = 4\pi^2\frac{m}{T^2}$$

where:

$$m$$

is the mass,

$$T$$

is the oscillation period,

$$k$$

is the spring constant.

The user sets:

$$m$$

and its uncertainty:

$$u(m)$$

The periods are determined from recorded times:

$$T_i = t_{i+1} - t_i$$

The mean period is:

$$\bar{T}$$

The standard deviation is:

$$s_T$$

The uncertainty of the mean period is:

$$u(T) = \frac{s_T}{\sqrt{n}}$$

The frequency is:

$$f = \frac{1}{\bar{T}}$$

The uncertainty of frequency is:

$$u(f) = \frac{u(T)}{\bar{T}^2}$$

---

## Solution

### 1. Recording the Motion

The first press of the spacebar starts the oscillator motion and the stopwatch.

Each next press of the spacebar records the time when the mass passes through the minimum position.

The recorded times are:

$$t_1,\ t_2,\ t_3,\ \dots,\ t_n$$

---

### 2. Period Calculation

The periods are calculated as:

$$T_i = t_{i+1} - t_i$$

---

### 3. Mean Period

The mean period is:

$$\bar{T} = \frac{T_1 + T_2 + \dots + T_n}{n}$$

---

### 4. Standard Deviation

The standard deviation of the periods is:

$$s_T = \sqrt{\frac{\sum (T_i - \bar{T})^2}{n - 1}}$$

---

### 5. Uncertainty of the Mean Period

The uncertainty of the mean period is:

$$u(T) = \frac{s_T}{\sqrt{n}}$$

---

### 6. Frequency

The frequency is calculated as:

$$f = \frac{1}{\bar{T}}$$

The uncertainty of frequency is:

$$u(f) = \frac{u(T)}{\bar{T}^2}$$

---

### 7. Spring Constant

The spring constant is calculated using:

$$k = 4\pi^2\frac{m}{\bar{T}^2}$$

---

### 8. Propagation of Uncertainty

The uncertainty of the spring constant is:

$$u(k) = \sqrt{\left(\frac{\partial k}{\partial m}u(m)\right)^2 + \left(\frac{\partial k}{\partial T}u(T)\right)^2}$$

The partial derivatives are:

$$\frac{\partial k}{\partial m} = \frac{4\pi^2}{T^2}$$

$$\frac{\partial k}{\partial T} = -\frac{8\pi^2m}{T^3}$$

Therefore:

$$u(k) = \sqrt{\left(\frac{4\pi^2}{T^2}u(m)\right)^2 + \left(\frac{8\pi^2m}{T^3}u(T)\right)^2}$$

---

## Final Result

The application displays:

$$k = \hat{k} \pm u(k)$$

It also displays the percentage uncertainty contributions from:

$$m$$

and:

$$T$$

---

## Conclusion

The application measures the spring constant of a mass-spring oscillator.

The oscillation period is obtained from repeated spacebar presses.

At least 10 periods should be recorded.

The program calculates the mean period, standard deviation, uncertainty of the mean period, frequency, uncertainty of frequency, spring constant, and uncertainty of spring constant.

The final result is written as:

$$k = \hat{k} \pm u(k)$$

The uncertainty contribution shows whether the main error comes from the mass measurement or the period measurement.
