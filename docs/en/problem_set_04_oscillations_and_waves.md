# Problem 5 – Superposition of waves, beats, and group velocity

## Given

Two harmonic waves are given:

$y_1(x,t) = A \sin(kx - \omega t)$

$y_2(x,t) = A \sin\big(kx - (\omega + \Delta \omega)t\big)$

We need to:

1. Determine the resultant wave $y = y_1 + y_2$ and write it in product form.
2. Find the beat frequency and the beat period at $x = 0$.
3. Interpret physically the envelope and the carrier wave.

---

## Solution

### 1. Resultant wave

The total wave is:

$y = y_1 + y_2$

Substitute:

$y = A\sin(kx - \omega t) + A\sin\big(kx - (\omega + \Delta \omega)t\big)$

Use identity:

$\sin\alpha + \sin\beta = 2\sin\left(\frac{\alpha+\beta}{2}\right)\cos\left(\frac{\alpha-\beta}{2}\right)$

Let:

$\alpha = kx - \omega t$

$\beta = kx - (\omega + \Delta \omega)t$

Then:

$\frac{\alpha+\beta}{2} = kx - \omega t - \frac{\Delta \omega}{2}t$

$\frac{\alpha-\beta}{2} = \frac{\Delta \omega}{2}t$

So:

$y = 2A \sin\left(kx - \omega t - \frac{\Delta \omega}{2}t\right)\cos\left(\frac{\Delta \omega}{2}t\right)$

Final product form:

$\boxed{y = 2A \cos\left(\frac{\Delta \omega}{2}t\right)\sin\left(kx - \omega t - \frac{\Delta \omega}{2}t\right)}$

---

### 2. Beat frequency

Frequencies:

$f_1 = \frac{\omega}{2\pi}$  
$f_2 = \frac{\omega + \Delta \omega}{2\pi}$  

Beat frequency:

$f_b = |f_2 - f_1| = \frac{\Delta \omega}{2\pi}$

$\boxed{f_b = \frac{\Delta \omega}{2\pi}}$

---

### 3. Beat period

$T_b = \frac{1}{f_b}$

$T_b = \frac{2\pi}{\Delta \omega}$

$\boxed{T_b = \frac{2\pi}{\Delta \omega}}$

---

### 4. Interpretation

Envelope:

$2A \cos\left(\frac{\Delta \omega}{2}t\right)$

Carrier wave:

$\sin\left(kx - \omega t - \frac{\Delta \omega}{2}t\right)$

- Envelope → slow amplitude change (beats)  
- Carrier → fast oscillation  

---

## Final Answer

$y = 2A \cos\left(\frac{\Delta \omega}{2}t\right)\sin\left(kx - \omega t - \frac{\Delta \omega}{2}t\right)$

$f_b = \frac{\Delta \omega}{2\pi}$

$T_b = \frac{2\pi}{\Delta \omega}$

---

## Conclusion

The superposition of two waves with close frequencies produces beats.  
The result is a fast oscillating carrier wave modulated by a slow envelope.
