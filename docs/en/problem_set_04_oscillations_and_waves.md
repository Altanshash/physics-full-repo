# Problem 5 – Superposition of waves, beats

## Given

Two harmonic waves:

$$
y_1(x,t) = A \sin(kx - \omega t)
$$

$$
y_2(x,t) = A \sin\big(kx - (\omega + \Delta \omega)t\big)
$$

---

## Solution

### 1. Resultant wave

Total wave:

$$
y = y_1 + y_2
$$

Substitute:

$$
y = A\sin(kx - \omega t) + A\sin\big(kx - (\omega + \Delta \omega)t\big)
$$

Use identity:

$$
\sin\alpha + \sin\beta =
2\sin\left(\frac{\alpha+\beta}{2}\right)
\cos\left(\frac{\alpha-\beta}{2}\right)
$$

Let:

$$
\alpha = kx - \omega t
$$

$$
\beta = kx - (\omega + \Delta \omega)t
$$

Now calculate:

$$
\frac{\alpha+\beta}{2} = kx - \omega t - \frac{\Delta \omega}{2}t
$$

$$
\frac{\alpha-\beta}{2} = \frac{\Delta \omega}{2}t
$$

Final result:

$$
\boxed{
y = 2A \cos\left(\frac{\Delta \omega}{2}t\right)
\sin\left(kx - \omega t - \frac{\Delta \omega}{2}t\right)
}
$$

---

### 2. Beat frequency

$$
f_1 = \frac{\omega}{2\pi}, \quad
f_2 = \frac{\omega + \Delta \omega}{2\pi}
$$

$$
f_b = |f_2 - f_1|
$$

$$
\boxed{
f_b = \frac{\Delta \omega}{2\pi}
}
$$

---

### 3. Beat period

$$
T_b = \frac{1}{f_b}
$$

$$
\boxed{
T_b = \frac{2\pi}{\Delta \omega}
}
$$

---

### 4. Interpretation

Envelope:

$$
2A \cos\left(\frac{\Delta \omega}{2}t\right)
$$

Carrier wave:

$$
\sin\left(kx - \omega t - \frac{\Delta \omega}{2}t\right)
$$

- Envelope → slow amplitude change (beats)  
- Carrier → fast oscillation  

---

## Final Answer

$$
y = 2A \cos\left(\frac{\Delta \omega}{2}t\right)
\sin\left(kx - \omega t - \frac{\Delta \omega}{2}t\right)
$$

$$
f_b = \frac{\Delta \omega}{2\pi}
$$

$$
T_b = \frac{2\pi}{\Delta \omega}
$$
