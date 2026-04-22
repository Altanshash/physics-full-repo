# Problem 5 – Superposition of waves, beats, and group velocity

## Given

Two harmonic waves are given:

$$
y_1(x,t) = A\sin(kx - \omega t)
$$

$$
y_2(x,t) = A\sin\big(kx - (\omega + \Delta\omega)t\big)
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
y = A\sin(kx - \omega t) + A\sin\big(kx - (\omega + \Delta\omega)t\big)
$$

Factor out $A$:

$$
y = A\left[\sin(kx - \omega t) + \sin\big(kx - (\omega + \Delta\omega)t\big)\right]
$$

Now use the trigonometric identity:

$$
\sin \alpha + \sin \beta = 2\sin\left(\frac{\alpha+\beta}{2}\right)\cos\left(\frac{\alpha-\beta}{2}\right)
$$

Let

$$
\alpha = kx - \omega t
$$

and

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
y = 2A\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)\cos\left(\frac{\Delta\omega}{2}t\right)
$$

So, the resultant wave in product form is

$$
\boxed{
y = 2A\cos\left(\frac{\Delta\omega}{2}t\right)\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)
}
$$

This can also be written as

$$
\boxed{
y = 2A\cos\left(\frac{\Delta\omega}{2}t\right)\sin\left(kx - \left(\omega + \frac{\Delta\omega}{2}\right)t\right)
}
$$

---

### 2. Beat frequency at $x = 0$

At the point $x = 0$, the wave becomes

$$
y(0,t) = 2A\cos\left(\frac{\Delta\omega}{2}t\right)\sin\left(-\omega t - \frac{\Delta\omega}{2}t\right)
$$

The beat phenomenon is determined by the slowly varying factor

$$
\cos\left(\frac{\Delta\omega}{2}t\right)
$$

The two ordinary frequencies are

$$
f_1 = \frac{\omega}{2\pi}
$$

$$
f_2 = \frac{\omega + \Delta\omega}{2\pi}
$$

So the beat frequency is the difference:

$$
f_b = |f_2 - f_1|
$$

$$
f_b = \left|\frac{\omega + \Delta\omega}{2\pi} - \frac{\omega}{2\pi}\right|
$$

$$
f_b = \frac{\Delta\omega}{2\pi}
$$

Thus,

$$
\boxed{f_b = \frac{\Delta\omega}{2\pi}}
$$

---

### 3. Beat period

The beat period is the reciprocal of the beat frequency:

$$
T_b = \frac{1}{f_b}
$$

Substitute the value of $f_b$:

$$
T_b = \frac{1}{\Delta\omega/(2\pi)}
$$

Hence,

$$
\boxed{T_b = \frac{2\pi}{\Delta\omega}}
$$

---

### 4. Physical interpretation

From the product form

$$
y = 2A\cos\left(\frac{\Delta\omega}{2}t\right)\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)
$$

we identify two parts:

#### Envelope

$$
\boxed{2A\cos\left(\frac{\Delta\omega}{2}t\right)}
$$

This term changes slowly with time and controls the amplitude of the total wave.  
It describes how the sound or oscillation becomes stronger and weaker.  
This is the **beat envelope**.

#### Carrier wave

$$
\boxed{\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)}
$$

This is the rapidly oscillating part inside the envelope.  
It describes the main fast wave motion.

So physically:

- the **envelope** describes the slow modulation of amplitude,
- the **carrier wave** describes the fast oscillation.

When the envelope is large, the interference is constructive.  
When the envelope is zero, the interference is destructive.

---

## Final Answer

The resultant wave is

$$
\boxed{
y = 2A\cos\left(\frac{\Delta\omega}{2}t\right)\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)
}
$$

The beat frequency at $x = 0$ is

$$
\boxed{f_b = \frac{\Delta\omega}{2\pi}}
$$

The beat period is

$$
\boxed{T_b = \frac{2\pi}{\Delta\omega}}
$$

The envelope is

$$
\boxed{2A\cos\left(\frac{\Delta\omega}{2}t\right)}
$$

The carrier wave is

$$
\boxed{\sin\left(kx - \omega t - \frac{\Delta\omega}{2}t\right)}
$$

---

## Conclusion

The superposition of two harmonic waves with slightly different angular frequencies produces beats.  
The resultant wave can be written as the product of a slowly varying envelope and a rapidly oscillating carrier wave.  
The envelope determines the amplitude modulation, while the carrier wave describes the fast oscillation.  
The beat frequency is

$$
\boxed{f_b = \frac{\Delta\omega}{2\pi}}
$$

and the beat period is

$$
\boxed{T_b = \frac{2\pi}{\Delta\omega}}
$$
