# Problem 6 – Rod on Metal Rails in a Magnetic Field

## Problem Statement

We have two conducting parallel rails separated by distance $L$.  
A conducting rod slides without friction along the rails and closes the circuit.

The whole circuit has resistance $R$.

A uniform magnetic field $\vec{B}$ is perpendicular to the plane of the rails.

For example data:

$$
m = 0.20\ \text{kg}
$$

$$
L = 0.30\ \text{m}
$$

$$
B = 0.80\ \text{T}
$$

$$
R = 0.50\ \Omega
$$

$$
\alpha = 25^\circ
$$

$$
g = 9.81\ \text{m/s}^2
$$

Answer the following questions:

1. Determine the motional EMF $\mathcal{E}(v)$ and the current $I(v)$.
2. Show that a magnetic braking force acts on the rod along the rails.
3. Write the equation of motion on the incline and reduce it to a form with damping proportional to $v$.
4. Determine the terminal velocity $v_\infty$.
5. Perform a power balance and show that in steady state:

$$
mg\sin\alpha \cdot v = I^2R
$$

---

## Given

$$
m = 0.20\ \text{kg}
$$

$$
L = 0.30\ \text{m}
$$

$$
B = 0.80\ \text{T}
$$

$$
R = 0.50\ \Omega
$$

$$
\alpha = 25^\circ
$$

$$
g = 9.81\ \text{m/s}^2
$$

---

## Solution

## 1. Motional EMF and Current

The motional EMF in the moving rod is:

$$
\mathcal{E}(v) = BLv
$$

The current in the circuit is:

$$
I(v) = \frac{\mathcal{E}(v)}{R}
$$

So:

$$
I(v) = \frac{BLv}{R}
$$

---

## 2. Magnetic Braking Force

The magnetic force on a current-carrying rod is:

$$
F_B = ILB
$$

Substitute:

$$
I = \frac{BLv}{R}
$$

Then:

$$
F_B = \frac{BLv}{R}LB
$$

$$
F_B = \frac{B^2L^2}{R}v
$$

This force is directed opposite to the motion.

Therefore, it is a magnetic braking force:

$$
F_{\text{brake}} = -\frac{B^2L^2}{R}v
$$

---

## 3. Equation of Motion

The component of gravity along the incline is:

$$
F_g = mg\sin\alpha
$$

The magnetic braking force is:

$$
F_{\text{brake}} = \frac{B^2L^2}{R}v
$$

Using Newton's second law:

$$
m\frac{dv}{dt} = mg\sin\alpha - \frac{B^2L^2}{R}v
$$

Divide by $m$:

$$
\frac{dv}{dt} = g\sin\alpha - \frac{B^2L^2}{mR}v
$$

This has the form:

$$
\frac{dv}{dt} = a_0 - kv
$$

where:

$$
a_0 = g\sin\alpha
$$

and

$$
k = \frac{B^2L^2}{mR}
$$

---

## 4. Terminal Velocity

At terminal velocity:

$$
\frac{dv}{dt} = 0
$$

So:

$$
mg\sin\alpha = \frac{B^2L^2}{R}v_\infty
$$

Therefore:

$$
v_\infty = \frac{mgR\sin\alpha}{B^2L^2}
$$

Substitute values:

$$
v_\infty =
\frac{0.20 \cdot 9.81 \cdot 0.50 \cdot \sin25^\circ}
{(0.80)^2(0.30)^2}
$$

$$
v_\infty =
\frac{0.20 \cdot 9.81 \cdot 0.50 \cdot 0.423}
{0.64 \cdot 0.09}
$$

$$
v_\infty =
\frac{0.415}{0.0576}
$$

$$
v_\infty \approx 7.21\ \text{m/s}
$$

---

## 5. Power Balance

In steady state, the rod moves with constant velocity:

$$
v = v_\infty
$$

The gravitational power is:

$$
P_g = mg\sin\alpha \cdot v
$$

The electric power converted into heat is:

$$
P_R = I^2R
$$

In steady state:

$$
P_g = P_R
$$

Therefore:

$$
mg\sin\alpha \cdot v = I^2R
$$

This means gravitational energy is converted into Joule heat.

---

## Final Conclusion

The motional EMF is:

$$
\mathcal{E}(v) = BLv
$$

The current is:

$$
I(v) = \frac{BLv}{R}
$$

The magnetic braking force is:

$$
F_{\text{brake}} = -\frac{B^2L^2}{R}v
$$

The equation of motion is:

$$
m\frac{dv}{dt} = mg\sin\alpha - \frac{B^2L^2}{R}v
$$

The terminal velocity is:

$$
v_\infty = \frac{mgR\sin\alpha}{B^2L^2}
$$

For the given values:

$$
v_\infty \approx 7.21\ \text{m/s}
$$

In steady state:

$$
mg\sin\alpha \cdot v = I^2R
$$

So gravitational energy is converted into Joule heat.
