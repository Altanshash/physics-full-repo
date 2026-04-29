# Problem 2 – Velocity Selection (Crossed Fields)

## Problem Statement

Crossed electric and magnetic fields can be used to select particles with a specific velocity.

Assume we have:

$$
\vec{E} = (0,E,0)
$$

$$
\vec{B} = (0,0,B)
$$

Answer the following questions:

1. Derive the condition for rectilinear motion.
2. Calculate $v_d$ for $E = 400\ \text{V/m}$ and $B = 0.8\ \text{T}$.
3. Does the kinetic energy change in steady motion?
4. Interpret the operating principle of the velocity selector.

---

## Given

$$
\vec{E} = (0,E,0)
$$

$$
\vec{B} = (0,0,B)
$$

$$
E = 400\ \text{V/m}
$$

$$
B = 0.8\ \text{T}
$$

---

## Solution

## 1. Condition for Rectilinear Motion

The total Lorentz force is:

$$
\vec{F} = q\vec{E} + q(\vec{v} \times \vec{B})
$$

For rectilinear motion, the particle must move in a straight line.

This means the total force must be zero:

$$
\vec{F} = 0
$$

So:

$$
q\vec{E} + q(\vec{v} \times \vec{B}) = 0
$$

Divide by $q$:

$$
\vec{E} + \vec{v} \times \vec{B} = 0
$$

Therefore:

$$
\vec{E} = - \vec{v} \times \vec{B}
$$

If the particle moves along the $x$-axis, then:

$$
\vec{v} = (v,0,0)
$$

Now calculate the cross product:

$$
\vec{v} \times \vec{B} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
v & 0 & 0 \\
0 & 0 & B
\end{vmatrix}
$$

$$
\vec{v} \times \vec{B} = (0,-vB,0)
$$

The electric force is directed along the $y$-axis:

$$
\vec{E} = (0,E,0)
$$

For straight motion:

$$
(0,E,0) + (0,-vB,0) = 0
$$

So:

$$
E - vB = 0
$$

Therefore, the required velocity is:

$$
v_d = \frac{E}{B}
$$

---

## 2. Calculate the Selected Velocity

Given:

$$
E = 400\ \text{V/m}
$$

$$
B = 0.8\ \text{T}
$$

Using the formula:

$$
v_d = \frac{E}{B}
$$

Substitute the values:

$$
v_d = \frac{400}{0.8}
$$

$$
v_d = 500\ \text{m/s}
$$

---

## 3. Does the Kinetic Energy Change?

In steady rectilinear motion:

$$
\vec{F} = 0
$$

So the acceleration is zero:

$$
a = 0
$$

The velocity remains constant:

$$
v = \text{constant}
$$

Kinetic energy is:

$$
K = \frac{1}{2}mv^2
$$

Since $v$ does not change, kinetic energy also does not change.

Therefore:

$$
\Delta K = 0
$$

The kinetic energy does **not** change.

---

## 4. Operating Principle of the Velocity Selector

A velocity selector uses crossed electric and magnetic fields.

The electric force is:

$$
\vec{F}_E = q\vec{E}
$$

The magnetic force is:

$$
\vec{F}_B = q(\vec{v} \times \vec{B})
$$

For particles with velocity:

$$
v = \frac{E}{B}
$$

the electric and magnetic forces are equal in magnitude and opposite in direction:

$$
F_E = F_B
$$

$$
qE = qvB
$$

Such particles move straight through the selector.

Particles with different velocities do not satisfy this condition, so they are deflected.

---

## Final Conclusion

The condition for rectilinear motion is:

$$
\vec{E} + \vec{v} \times \vec{B} = 0
$$

The selected velocity is:

$$
v_d = \frac{E}{B}
$$

For the given values:

$$
v_d = 500\ \text{m/s}
$$

In steady motion, the kinetic energy does **not** change:

$$
\Delta K = 0
$$

The velocity selector allows only particles with velocity

$$
v = \frac{E}{B}
$$

to pass straight through without deflection.
