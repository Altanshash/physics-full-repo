# Problem 7 – Loop Pulled into a Magnetic Field Region

## Problem Statement

A rectangular conducting loop with resistance $R$ has dimensions $a \times b$.

It is pulled with constant velocity $v$ into a region of uniform magnetic field $B$ perpendicular to the loop.

For example data:

$$
a = 0.20\ \text{m}
$$

$$
b = 0.10\ \text{m}
$$

$$
B = 0.60\ \text{T}
$$

$$
R = 0.40\ \Omega
$$

$$
v = 1.5\ \text{m/s}
$$

Answer the following questions:

1. Write down the flux $\Phi(t)$ in the entering phase.
2. Determine $\mathcal{E}$ and $I$ in this phase.
3. Determine the braking force $F(v)$.
4. Calculate the mechanical power required to maintain constant $v$ and show that it is equal to thermal power $I^2R$.
5. What happens to the current when the loop is entirely in the uniform field?

---

## Given

$$
a = 0.20\ \text{m}
$$

$$
b = 0.10\ \text{m}
$$

$$
B = 0.60\ \text{T}
$$

$$
R = 0.40\ \Omega
$$

$$
v = 1.5\ \text{m/s}
$$

---

## Solution

## 1. Magnetic Flux During Entering Phase

During the entering phase, only part of the loop is inside the magnetic field.

Let the loop enter the field along the side $a$.

The distance inside the magnetic field is:

$$
x(t) = vt
$$

The area inside the magnetic field is:

$$
A(t) = b x(t)
$$

Substitute $x(t) = vt$:

$$
A(t) = bvt
$$

Magnetic flux is:

$$
\Phi(t) = BA(t)
$$

Therefore:

$$
\Phi(t) = Bbvt
$$

This formula is valid for:

$$
0 \le vt \le a
$$

or

$$
0 \le t \le \frac{a}{v}
$$

---

## 2. Induced EMF and Current

According to Faraday's law:

$$
\mathcal{E} = -\frac{d\Phi}{dt}
$$

Substitute:

$$
\Phi(t) = Bbvt
$$

Then:

$$
\mathcal{E} = -\frac{d}{dt}(Bbvt)
$$

Since $B$, $b$, and $v$ are constants:

$$
\mathcal{E} = -Bbv
$$

The magnitude is:

$$
|\mathcal{E}| = Bbv
$$

Substitute the values:

$$
|\mathcal{E}| = 0.60 \cdot 0.10 \cdot 1.5
$$

$$
|\mathcal{E}| = 0.09\ \text{V}
$$

The current is:

$$
I = \frac{|\mathcal{E}|}{R}
$$

Substitute:

$$
I = \frac{0.09}{0.40}
$$

$$
I = 0.225\ \text{A}
$$

---

## 3. Braking Force

The magnetic force on the vertical side of the loop inside the magnetic field is:

$$
F = I b B
$$

Substitute:

$$
I = \frac{Bbv}{R}
$$

Then:

$$
F(v) = \frac{Bbv}{R} \cdot bB
$$

$$
F(v) = \frac{B^2 b^2 v}{R}
$$

Substitute the values:

$$
F = \frac{(0.60)^2(0.10)^2(1.5)}{0.40}
$$

$$
F = \frac{0.36 \cdot 0.01 \cdot 1.5}{0.40}
$$

$$
F = \frac{0.0054}{0.40}
$$

$$
F = 0.0135\ \text{N}
$$

This force acts opposite to the motion.

---

## 4. Mechanical Power and Thermal Power

The mechanical power required to maintain constant velocity is:

$$
P_{\text{mech}} = Fv
$$

Substitute:

$$
P_{\text{mech}} = 0.0135 \cdot 1.5
$$

$$
P_{\text{mech}} = 0.02025\ \text{W}
$$

The thermal power is:

$$
P_{\text{thermal}} = I^2R
$$

Substitute:

$$
P_{\text{thermal}} = (0.225)^2 \cdot 0.40
$$

$$
P_{\text{thermal}} = 0.050625 \cdot 0.40
$$

$$
P_{\text{thermal}} = 0.02025\ \text{W}
$$

Therefore:

$$
P_{\text{mech}} = P_{\text{thermal}}
$$

or:

$$
Fv = I^2R
$$

---

## 5. Current When the Loop Is Entirely in the Field

When the loop is completely inside the uniform magnetic field, the magnetic flux becomes constant:

$$
\Phi = BS
$$

Since the flux does not change:

$$
\frac{d\Phi}{dt} = 0
$$

Therefore:

$$
\mathcal{E} = 0
$$

and

$$
I = 0
$$

So, when the loop is entirely in the uniform magnetic field, the current disappears.

---

## Final Conclusion

During the entering phase, the magnetic flux is:

$$
\Phi(t) = Bbvt
$$

The induced EMF is:

$$
|\mathcal{E}| = Bbv
$$

For the given values:

$$
|\mathcal{E}| = 0.09\ \text{V}
$$

The current is:

$$
I = 0.225\ \text{A}
$$

The braking force is:

$$
F(v) = \frac{B^2b^2v}{R}
$$

For the given values:

$$
F = 0.0135\ \text{N}
$$

The mechanical power is:

$$
P_{\text{mech}} = 0.02025\ \text{W}
$$

The thermal power is:

$$
I^2R = 0.02025\ \text{W}
$$

So:

$$
P_{\text{mech}} = I^2R
$$

When the loop is completely inside the magnetic field:

$$
I = 0
$$
