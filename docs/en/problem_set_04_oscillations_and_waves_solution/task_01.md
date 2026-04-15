# Problem Set 4
## Problem 1 – Harmonic motion: motion parameters

### Given

A function describing harmonic motion is given:

`x(t) = A cos(ωt + φ)`

Find:

1. the period `T` and the frequency `f`;
2. the maximum velocity `v_max` and the maximum acceleration `a_max`;
3. for `A = 0.2 m`, `f = 2 Hz`:
   - calculate `ω`,
   - calculate `v_max`,
   - calculate `a_max`.

---

## Solution

### 1. Period and frequency

For harmonic motion, angular frequency, period, and frequency are related by:

`ω = 2πf`

From this:

`f = ω / (2π)`

Since period is the inverse of frequency:

`T = 1 / f`

Substituting `f = ω / (2π)`:

`T = 2π / ω`

### Answer:

`T = 2π / ω`

`f = ω / (2π)`

---

### 2. Maximum velocity

Velocity is the first derivative of displacement with respect to time:

`v(t) = dx/dt`

Given:

`x(t) = A cos(ωt + φ)`

Differentiate:

`v(t) = -Aω sin(ωt + φ)`

The maximum value of `sin(ωt + φ)` in absolute value is 1, therefore:

`v_max = Aω`

### Answer:

`v_max = Aω`

---

### 3. Maximum acceleration

Acceleration is the derivative of velocity:

`a(t) = dv/dt`

From

`v(t) = -Aω sin(ωt + φ)`

differentiate again:

`a(t) = -Aω² cos(ωt + φ)`

The maximum value of `cos(ωt + φ)` in absolute value is 1, therefore:

`a_max = Aω²`

### Answer:

`a_max = Aω²`

---

## Numerical calculations

Given:

`A = 0.2 m`

`f = 2 Hz`

### 1. Calculate `ω`

Use the formula:

`ω = 2πf`

Substitute the values:

`ω = 2π * 2 = 4π rad/s`

Using `π ≈ 3.14`:

`ω ≈ 4 * 3.14 = 12.56 rad/s`

### 2. Calculate `v_max`

Use:

`v_max = Aω`

Substitute the values:

`v_max = 0.2 * 12.56`

`v_max = 2.512 m/s`

So:

`v_max ≈ 2.51 m/s`

### 3. Calculate `a_max`

Use:

`a_max = Aω²`

Substitute the values:

`a_max = 0.2 * (12.56)^2`

First calculate:

`(12.56)^2 = 157.75`

Then:

`a_max = 0.2 * 157.75 = 31.55 m/s²`

So:

`a_max ≈ 31.55 m/s²`

---

## Final Answer

`T = 2π / ω`

`f = ω / (2π)`

`v_max = Aω`

`a_max = Aω²`

For `A = 0.2 m` and `f = 2 Hz`:

`ω = 4π ≈ 12.56 rad/s`

`v_max ≈ 2.51 m/s`

`a_max ≈ 31.55 m/s²`

---

## Conclusion

In harmonic motion, the period and frequency are determined by angular frequency:

`T = 2π / ω`

`f = ω / (2π)`

The maximum velocity is:

`v_max = Aω`

The maximum acceleration is:

`a_max = Aω²`

For `A = 0.2 m` and `f = 2 Hz`, the angular frequency is `12.56 rad/s`, the maximum velocity is `2.51 m/s`, and the maximum acceleration is `31.55 m/s²`.
