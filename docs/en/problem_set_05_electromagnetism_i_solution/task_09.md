# Problem 9 – Dipole in an External Field

## Given

A dipole is placed in a uniform external electric field:

```math
\vec{E}_0
```

The electric dipole moment is:

```math
\vec{p}
```

Find:

1. Formula for the torque acting on the dipole
2. Potential energy of the dipole
3. Equation of angular motion
4. Linearized equation for small displacements
5. Interpretation as a harmonic oscillator

---

## Solution

## 1. Torque acting on the dipole

For an electric dipole in a uniform electric field, the torque is:

```math
\vec{\tau}
=
\vec{p}\times\vec{E}_0
```

Magnitude of torque:

```math
\tau
=
pE_0\sin\theta
```

Here, $\theta$ is the angle between $\vec{p}$ and $\vec{E}_0$.

---

## 2. Potential energy of the dipole

Potential energy of a dipole in an electric field is:

```math
U
=
-\vec{p}\cdot\vec{E}_0
```

Using the dot product:

```math
U(\theta)
=
-pE_0\cos\theta
```

Minimum energy occurs when:

```math
\theta=0
```

So the dipole is stable when it is aligned with the field.

---

## 3. Equation of angular motion

Rotational equation of motion:

```math
I\frac{d^2\theta}{dt^2}
=
\tau
```

The torque acts to reduce the angle $\theta$, therefore:

```math
I\frac{d^2\theta}{dt^2}
=
-pE_0\sin\theta
```

So:

```math
\frac{d^2\theta}{dt^2}
+
\frac{pE_0}{I}\sin\theta
=
0
```

---

## 4. Small-angle approximation

For small angles:

```math
\sin\theta \approx \theta
```

Then:

```math
\frac{d^2\theta}{dt^2}
+
\frac{pE_0}{I}\theta
=
0
```

This is the equation of simple harmonic motion.

---

## 5. Harmonic oscillator interpretation

The standard harmonic oscillator equation is:

```math
\frac{d^2\theta}{dt^2}
+
\omega^2\theta
=
0
```

Comparing:

```math
\omega^2
=
\frac{pE_0}{I}
```

Therefore:

```math
\omega
=
\sqrt{\frac{pE_0}{I}}
```

The period of small oscillations is:

```math
T
=
2\pi\sqrt{\frac{I}{pE_0}}
```

---

## Final Answer

```math
\vec{\tau}
=
\vec{p}\times\vec{E}_0
```

```math
\tau
=
pE_0\sin\theta
```

```math
U(\theta)
=
-pE_0\cos\theta
```

```math
\frac{d^2\theta}{dt^2}
+
\frac{pE_0}{I}\sin\theta
=
0
```

For small angles:

```math
\frac{d^2\theta}{dt^2}
+
\frac{pE_0}{I}\theta
=
0
```

```math
\omega
=
\sqrt{\frac{pE_0}{I}}
```

```math
T
=
2\pi\sqrt{\frac{I}{pE_0}}
```

---

## Conclusion

A dipole in a uniform electric field experiences a torque.  
This torque tries to align the dipole with the field.  
The potential energy is minimum when the dipole is parallel to the electric field.  
For small angular displacements, the dipole behaves like a harmonic oscillator.
