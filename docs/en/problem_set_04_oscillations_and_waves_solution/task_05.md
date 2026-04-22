# Problem 5 – Superposition of waves, beats, and group velocity

## Given

Two harmonic waves are given:

$$
y_1(x,t) = A \sin(kx - \omega t)
$$

$$
y_2(x,t) = A \sin\big(kx - (\omega + \Delta \omega)t\big)
$$

We need to:

1. Determine the resultant wave $y = y_1 + y_2$ and reduce it to product form (carrier × envelope).
2. Identify the beat frequency and the beat period at the point $x = 0$.
3. Interpret physically what the envelope describes and what the carrier wave describes.

---

## Solution

### 1. Resultant wave

The total wave is

$$
y = y_1 + y_2
$$

Substitute the given functions:

$$
y = A \sin(kx - \omega t) + A \sin\big(kx - (\omega + \Delta\omega)t\big)
$$

Factor out $A$:

$$
y = A\left[\sin(kx - \omega t) + \sin\big(kx - (\omega + \Delta\omega)t\big)\right]
$$

Now use the trigonometric identity

$$
\sin \alpha + \sin \beta = 2 \sin\left(\frac{\alpha+\beta}{2}\right)\cos\left(\frac{\alpha-\beta}{2}\right)
$$

Let

$$
\alpha = kx - \omega t
$$

$$
\beta = kx - (\omega + \Delta\omega)t
$$

Then

$$
\frac{\alpha+\beta}{2}
=
\frac{(kx-\omega t) + \big(kx-(\omega+\Delta\omega)t\big)}{2}
$$

$$
\frac{\alpha+\beta}{2}
=
\frac{2kx - 2\omega t - \Delta\omega t}{2}
$$

$$
\frac{\alpha+\beta}{2}
=
kx - \omega t - \frac{\Delta\omega}{2}t
$$

Also,

$$
\frac{\alpha-\beta}{2}
=
\frac{(kx-\omega t) - \big(kx-(\omega+\Delta\omega)t\big)}{2}
$$

$$
\frac{\alpha-\beta}{2}
=
\frac{\Delta\omega t}{2}
$$

Therefore,

$$
y = 2A \sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)
\cos\left(\frac{\Delta\omega}{2}t\right)
$$

So the product form is

$$
\boxed{
y = 2A \cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)
}
$$

---

### 2. Carrier wave and envelope

From the product form

$$
y = 2A \cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)
$$

we can identify:

#### Envelope

$$
\boxed{
2A \cos\left(\frac{\Delta\omega}{2}t\right)
}
$$

This term changes slowly with time and controls the amplitude of the total wave.

#### Carrier wave

$$
\boxed{
\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)
}
$$

This is the fast oscillating part inside the envelope.

---

### 3. Beat frequency at $x = 0$

At the point $x = 0$:

$$
y(0,t) = 2A \cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(-\omega t - \frac{\Delta\omega}{2}t\right)
$$

The beats are determined by the envelope

$$
\cos\left(\frac{\Delta\omega}{2}t\right)
$$

The angular beat frequency is

$$
\boxed{\omega_b = \Delta\omega}
$$

Therefore, the beat frequency is

$$
\boxed{f_b = \frac{\Delta\omega}{2\pi}}
$$

---

### 4. Beat period

The beat period is the inverse of the beat frequency:

$$
T_b = \frac{1}{f_b}
$$

Substitute $f_b$:

$$
T_b = \frac{1}{\Delta\omega/(2\pi)}
$$

$$
\boxed{T_b = \frac{2\pi}{\Delta\omega}}
$$

---

## Interpretation

When two waves have almost equal frequencies, their superposition produces **beats**.

- The **carrier wave** is the fast oscillation.
- The **envelope** is the slowly varying amplitude.
- The envelope shows how the amplitude increases and decreases with time.
- When the envelope is maximum, the two waves interfere constructively.
- When the envelope is zero, the two waves interfere destructively.

So physically:

- the **carrier** describes the rapid wave oscillation,
- the **envelope** describes the slow modulation of amplitude, that is, the beat pattern.

---

## Final Answer

The resultant wave is

$$
\boxed{
y = 2A \cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)
}
$$

where:

- the **envelope** is

$$
\boxed{
2A \cos\left(\frac{\Delta\omega}{2}t\right)
}
$$

- the **carrier wave** is

$$
\boxed{
\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)
}
$$

The beat frequency is

$$
\boxed{
f_b = \frac{\Delta\omega}{2\pi}
}
$$

The beat period is

$$
\boxed{
T_b = \frac{2\pi}{\Delta\omega}
}
$$

---

## Conclusion

The sum of two harmonic waves with close frequencies can be written as the product of a fast oscillating carrier wave and a slow envelope. This produces the phenomenon of beats. The envelope determines the amplitude modulation, while the carrier represents the rapid oscillation of the wave.
