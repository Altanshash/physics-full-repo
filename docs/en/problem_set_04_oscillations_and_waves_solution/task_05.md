# Problem 5 – Superposition of waves, beats, and group velocity

## Given

Two harmonic waves are given:

$$
y_1(x,t) = A\sin(kx-\omega t)
$$

$$
y_2(x,t) = A\sin\big(kx-(\omega+\Delta\omega)t\big)
$$

We need to:

1. Determine the resultant wave $y=y_1+y_2$ and write it in product form.
2. Find the beat frequency and the beat period at $x=0$.
3. Explain physically what the envelope and the carrier wave describe.

---

## Solution

### 1. Resultant wave

The total wave is

$$
y = y_1 + y_2
$$

Substitute the given functions:

$$
y = A\sin(kx-\omega t) + A\sin\big(kx-(\omega+\Delta\omega)t\big)
$$

Factor out $A$:

$$
y = A\left[\sin(kx-\omega t)+\sin\big(kx-(\omega+\Delta\omega)t\big)\right]
$$

Now use the identity

$$
\sin\alpha+\sin\beta
=
2\sin\left(\frac{\alpha+\beta}{2}\right)\cos\left(\frac{\alpha-\beta}{2}\right)
$$

Take

$$
\alpha = kx-\omega t
$$

$$
\beta = kx-(\omega+\Delta\omega)t
$$

Then

$$
\frac{\alpha+\beta}{2}
=
\frac{(kx-\omega t)+(kx-(\omega+\Delta\omega)t)}{2}
$$

$$
\frac{\alpha+\beta}{2}
=
\frac{2kx-2\omega t-\Delta\omega t}{2}
$$

$$
\frac{\alpha+\beta}{2}
=
kx-\omega t-\frac{\Delta\omega}{2}t
$$

Also,

$$
\frac{\alpha-\beta}{2}
=
\frac{(kx-\omega t)-(kx-(\omega+\Delta\omega)t)}{2}
$$

$$
\frac{\alpha-\beta}{2}
=
\frac{\Delta\omega\, t}{2}
$$

Therefore,

$$
y
=
2A\sin\left(kx-\omega t-\frac{\Delta\omega}{2}t\right)
\cos\left(\frac{\Delta\omega}{2}t\right)
$$

So the product form is

$$
\boxed{
y
=
2A\cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(kx-\omega t-\frac{\Delta\omega}{2}t\right)
}
$$

or equivalently,

$$
\boxed{
y
=
2A\cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(kx-\left(\omega+\frac{\Delta\omega}{2}\right)t\right)
}
$$

---

### 2. Envelope and carrier wave

From the product form,

$$
y
=
2A\cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(kx-\left(\omega+\frac{\Delta\omega}{2}\right)t\right)
$$

the **envelope** is

$$
\boxed{
2A\cos\left(\frac{\Delta\omega}{2}t\right)
}
$$

and the **carrier wave** is

$$
\boxed{
\sin\left(kx-\left(\omega+\frac{\Delta\omega}{2}\right)t\right)
}
$$

---

### 3. Beat frequency at $x=0$

At $x=0$,

$$
y(0,t)
=
2A\cos\left(\frac{\Delta\omega}{2}t\right)
\sin\left(-\left(\omega+\frac{\Delta\omega}{2}\right)t\right)
$$

The beats are determined by the slowly changing factor

$$
\cos\left(\frac{\Delta\omega}{2}t\right)
$$

The two ordinary frequencies are

$$
f_1=\frac{\omega}{2\pi}, \qquad
f_2=\frac{\omega+\Delta\omega}{2\pi}
$$

So the beat frequency is

$$
f_b = |f_2-f_1|
$$

$$
f_b
=
\left|
\frac{\omega+\Delta\omega}{2\pi}
-
\frac{\omega}{2\pi}
\right|
$$

$$
\boxed{
f_b=\frac{\Delta\omega}{2\pi}
}
$$

---

### 4. Beat period

The beat period is

$$
T_b=\frac{1}{f_b}
$$

Therefore,

$$
T_b=\frac{1}{\Delta\omega/(2\pi)}
$$

$$
\boxed{
T_b=\frac{2\pi}{\Delta\omega}
}
$$

---

## Interpretation

When two waves have the same wave number $k$ but slightly different angular frequencies, their sum produces **beats**.

- The **carrier wave** is the fast oscillation.
- The **envelope** describes how the amplitude changes slowly with time.
- When the envelope is large, the interference is constructive.
- When the envelope is zero, the interference is destructive.

In this problem, the envelope depends only on **time**, not on position $x$, because both waves have the same $k$.

So this is a beat phenomenon in time.

---

## Final Answer

The resultant wave is

$$
\boxed{
y
=
2A\cos\left(\frac{\Delta\omega}{2}t\right)
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
f_b=\frac{\Delta\omega}{2\pi}
}
$$

The beat period is

$$
\boxed{
T_b=\frac{2\pi}{\Delta\omega}
}
$$

---

## Conclusion

The superposition of two harmonic waves with equal wave number and slightly different frequencies produces beats. The resultant wave can be written as a product of a fast carrier wave and a slow envelope. The envelope shows the amplitude modulation in time, and the beat frequency is equal to the difference of the two frequencies.
