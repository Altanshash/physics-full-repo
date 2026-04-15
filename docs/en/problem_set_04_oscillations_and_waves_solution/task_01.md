# Problem Set 4  
## Problem 1 – Harmonic motion: motion parameters

### Given
Harmonic motion is described by the function:

\[
x(t) = A \cos(\omega t + \varphi)
\]

Find:

1. the period \(T\) and the frequency \(f\);
2. the maximum velocity \(v_{\max}\) and the maximum acceleration \(a_{\max}\);
3. for \(A = 0.2\ \text{m}\), \(f = 2\ \text{Hz}\):
   - calculate \(\omega\),
   - calculate \(v_{\max}\),
   - calculate \(a_{\max}\).

---

## Solution

### 1. Period and frequency

For harmonic motion, angular frequency \(\omega\), period \(T\), and frequency \(f\) are related by:

\[
\omega = 2\pi f
\]

and

\[
T = \frac{1}{f}
\]

Since

\[
f = \frac{\omega}{2\pi}
\]

then the period can also be written as:

\[
T = \frac{2\pi}{\omega}
\]

### Answer:
\[
T = \frac{2\pi}{\omega}, \qquad f = \frac{\omega}{2\pi}
\]

---

### 2. Maximum velocity

The velocity is the first derivative of displacement:

\[
v(t) = \frac{dx}{dt}
\]

Differentiate the given function:

\[
x(t) = A\cos(\omega t + \varphi)
\]

\[
v(t) = -A\omega \sin(\omega t + \varphi)
\]

The maximum value of \(\sin(\omega t + \varphi)\) in absolute value is 1, therefore the maximum velocity is:

\[
v_{\max} = A\omega
\]

### Answer:
\[
v_{\max} = A\omega
\]

---

### 3. Maximum acceleration

The acceleration is the derivative of velocity:

\[
a(t) = \frac{dv}{dt}
\]

Differentiate:

\[
v(t) = -A\omega \sin(\omega t + \varphi)
\]

\[
a(t) = -A\omega^2 \cos(\omega t + \varphi)
\]

The maximum value of \(\cos(\omega t + \varphi)\) in absolute value is 1, so:

\[
a_{\max} = A\omega^2
\]

### Answer:
\[
a_{\max} = A\omega^2
\]

---

## Numerical calculations

Given:

\[
A = 0.2\ \text{m}, \qquad f = 2\ \text{Hz}
\]

### 1. Calculate \(\omega\)

Use the formula:

\[
\omega = 2\pi f
\]

Substitute \(f = 2\ \text{Hz}\):

\[
\omega = 2\pi \cdot 2 = 4\pi\ \text{rad/s}
\]

\[
\omega \approx 12.57\ \text{rad/s}
\]

---

### 2. Calculate \(v_{\max}\)

Use:

\[
v_{\max} = A\omega
\]

Substitute the values:

\[
v_{\max} = 0.2 \cdot 12.57
\]

\[
v_{\max} \approx 2.51\ \text{m/s}
\]

---

### 3. Calculate \(a_{\max}\)

Use:

\[
a_{\max} = A\omega^2
\]

Substitute the values:

\[
a_{\max} = 0.2 \cdot (12.57)^2
\]

\[
a_{\max} = 0.2 \cdot 157.9
\]

\[
a_{\max} \approx 31.58\ \text{m/s}^2
\]

---

## Final Answer

\[
T = \frac{2\pi}{\omega}, \qquad f = \frac{\omega}{2\pi}
\]

\[
v_{\max} = A\omega
\]

\[
a_{\max} = A\omega^2
\]

For \(A = 0.2\ \text{m}\), \(f = 2\ \text{Hz}\):

\[
\omega = 4\pi \approx 12.57\ \text{rad/s}
\]

\[
v_{\max} \approx 2.51\ \text{m/s}
\]

\[
a_{\max} \approx 31.58\ \text{m/s}^2
\]

---

## Conclusion

In harmonic motion, the period and frequency are determined by the angular frequency:

\[
T = \frac{2\pi}{\omega}, \qquad f = \frac{\omega}{2\pi}
\]

The maximum velocity depends linearly on both amplitude and angular frequency:

\[
v_{\max} = A\omega
\]

The maximum acceleration depends on the amplitude and on the square of angular frequency:

\[
a_{\max} = A\omega^2
\]

For the given values \(A = 0.2\ \text{m}\) and \(f = 2\ \text{Hz}\), the body oscillates with angular frequency \(12.57\ \text{rad/s}\), reaches a maximum velocity of \(2.51\ \text{m/s}\), and a maximum acceleration of \(31.58\ \text{m/s}^2\).
