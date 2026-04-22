# Problem 5 – Superposition of waves, beats, and group velocity

## Given

Two harmonic waves are given:

$$
y_1(x,t) = A \sin(kx - \omega t)
$$

$$
y_2(x,t) = A \sin\big(kx - (\omega + \Delta\omega)t\big)
$$

We need to:

1. Determine the resultant wave $y = y_1 + y_2$ and reduce it to product form (carrier × envelope).
2. Identify the beat frequency and the beat period at the point $x = 0$.
3. Interpret physically what the envelope describes and what the carrier wave describes.

---

## Solution

### 1. Resultant wave in product form

The total wave is

$$
y = y_1 + y_2
$$

Substitute the given expressions:

$$
y = A\sin(kx-\omega t) + A\sin\big(kx-(\omega+\Delta\omega)t\big)
$$

Factor out $A$:

$$
y = A\left[\sin(kx-\omega t) + \sin\big(kx-(\omega+\Delta\omega)t\big)\right]
$$

Now use the trigonometric identity

$$
\sin\alpha + \sin\beta = 2\sin\left(\frac{\alpha+\beta}{2}\right)\cos\left(\frac{\alpha-\beta}{2}\right)
$$

Take

$$
\alpha = kx-\omega t
$$

$$
\beta = kx-(\omega+\Delta\omega)t
$$

First, calculate

$$
\frac{\alpha+\beta}{2}
=
\frac{(kx-\omega t) + (kx-(\omega+\Delta\omega)t)}{2}
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

Now calculate

$$
\frac{\alpha-\beta}{2}
=
\frac{(kx-\omega t) - (kx-(\omega+\Delta\omega)t)}{2}
$$

$$
\frac{\alpha-\beta}{2}
=
\frac{\Delta\omega t}{2}
$$

Therefore,

$$
y = 2A\sin\left(kx-\omega t-\frac{\Delta\omega}{2}t\right)\cos\left(\frac{\Delta\omega}{2}t\right)
$$

or equivalently,

$$
\boxed{
y = 2A\cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(kx-\left(\omega+\frac{\Delta\omega}{2}\right)t\right)
}
$$

This is the required product form.

---

### 2. Carrier wave and envelope

From the product form

$$
y = 2A\cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(kx-\left(\omega+\frac{\Delta\omega}{2}\right)t\right)
$$

we identify:

#### Envelope

$$
\boxed{
2A\cos\left(\frac{\Delta\omega}{2}t\right)
}
$$

This term changes slowly and determines the amplitude of the resultant wave.

#### Carrier wave

$$
\boxed{
\sin\left(kx-\left(\omega+\frac{\Delta\omega}{2}\right)t\right)
}
$$

This is the fast oscillating part of the wave.

---

### 3. Beat frequency at $x=0$

At $x=0$, the wave becomes

$$
y(0,t) =
2A\cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(-\left(\omega+\frac{\Delta\omega}{2}\right)t\right)
$$

The beats are produced by the envelope term

$$
\cos\left(\frac{\Delta\omega}{2}t\right)
$$

The two original frequencies are

$$
f_1 = \frac{\omega}{2\pi}
$$

$$
f_2 = \frac{\omega+\Delta\omega}{2\pi}
$$

So the beat frequency is the difference of frequencies:

$$
f_b = |f_2-f_1|
$$

$$
f_b = \frac{\Delta\omega}{2\pi}
$$

Hence,

$$
\boxed{
f_b = \frac{\Delta\omega}{2\pi}
}
$$

---

### 4. Beat period

The beat period is the reciprocal of the beat frequency:

$$
T_b = \frac{1}{f_b}
$$

Substitute $f_b$:

$$
T_b = \frac{1}{\Delta\omega/(2\pi)}
$$

Therefore,

$$
\boxed{
T_b = \frac{2\pi}{\Delta\omega}
}
$$

---

## Interpretation

When two waves with close frequencies are added, the result is not just another simple wave. The amplitude becomes time-dependent.

- The **carrier wave** is the fast oscillation.
- The **envelope** is the slow change of amplitude.
- The envelope shows the phenomenon of **beats**.
- Large amplitude means **constructive interference**.
- Small or zero amplitude means **destructive interference**.

So physically:

- the **carrier** describes the rapid oscillation of the wave,
- the **envelope** describes how the amplitude grows and decreases with time.

---

## Final Answer

The resultant wave is

$$
\boxed{
y = 2A\cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(kx-\left(\omega+\frac{\Delta\omega}{2}\right)t\right)
}
$$

The envelope is

$$
\boxed{
2A\cos\left(\frac{\Delta\omega}{2}t\right)
}
$$

The carrier wave is

$$
\boxed{
\sin\left(kx-\left(\omega+\frac{\Delta\omega}{2}\right)t\right)
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

The superposition of two harmonic waves with close frequencies produces beats. The resultant wave can be written as the product of a rapidly oscillating carrier wave and a slowly varying envelope. The envelope determines the beat pattern, and the beat frequency is equal to the difference of the two frequencies.
