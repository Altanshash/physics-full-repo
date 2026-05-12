# Problem 4 – Linear Regression and Determination of Gravity

## Given

Free fall model:

$$h = \frac{1}{2}gt^2$$

Height values:

$$h = [0.20,\ 0.40,\ 0.60,\ 0.80,\ 1.00]\ \text{m}$$

Time values:

$$t = [0.202,\ 0.287,\ 0.351,\ 0.404,\ 0.452]\ \text{s}$$

---

## Solution

### 1. Linear Form of the Model

The original equation is:

$$h = \frac{1}{2}gt^2$$

Let:

$$x = t^2$$

Then the equation becomes:

$$h = kx$$

where:

$$k = \frac{g}{2}$$

Therefore:

$$g = 2k$$

---

### 2. Calculate Values of x

Since:

$$x = t^2$$

we get:

$$x = [0.040804,\ 0.082369,\ 0.123201,\ 0.163216,\ 0.204304]$$

---

### 3. Linear Regression

For the model:

$$h = kx$$

the slope is calculated as:

$$k = \frac{\sum x_i h_i}{\sum x_i^2}$$

Substituting the data gives:

$$k = 4.8899$$

---

### 4. Determination of g

Since:

$$g = 2k$$

then:

$$g = 2 \cdot 4.8899$$

$$g = 9.7797\ \text{m/s}^2$$

Rounded:

$$g = 9.78\ \text{m/s}^2$$

---

### 5. Uncertainty of g

The uncertainty of the slope is:

$$u(k) = 0.0071$$

Since:

$$g = 2k$$

the uncertainty of g is:

$$u(g) = 2u(k)$$

$$u(g) = 2 \cdot 0.0071$$

$$u(g) = 0.014\ \text{m/s}^2$$

Rounded:

$$u(g) = 0.01\ \text{m/s}^2$$

---

### 6. Goodness of Fit

The coefficient of determination is:

$$R^2 = 0.99995$$

This value is very close to 1, which means that the linear model fits the experimental data very well.

---

## Final Result

$$g = 9.78 \pm 0.01\ \text{m/s}^2$$

---

## Conclusion

Using the free fall model and linear regression, the acceleration due to gravity was found to be:

$$g = 9.78 \pm 0.01\ \text{m/s}^2$$

The coefficient of determination is:

$$R^2 = 0.99995$$

Therefore, the experimental data fits the linear model very well, and the obtained value of gravity is close to the accepted value.
