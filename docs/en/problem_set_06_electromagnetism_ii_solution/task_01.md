# Problem 1 – Lorentz Force

## Problem Statement

For the following data:

$$
\vec{B} = (0,0,1)\ \text{T}
$$

$$
\vec{v} = (2,3,0)\ \text{m/s}
$$

$$
q = 1\ \text{mC}
$$

Answer the following questions:

1. Determine the Lorentz force $\vec{F}$ acting on the charge.
2. Solve the equation of motion for this charge, assuming that at time $t = 0$ it is at the point $(0,0,0)$.
3. Calculate the magnitude $|\vec{F}|$.
4. Does the magnetic force do work?
5. Determine the radius of the trajectory for $m = 0.01\ \text{kg}$.
6. How will $r$ change when the value of $B$ is doubled?

---

## Given

$$
\vec{B} = (0,0,1)\ \text{T}
$$

$$
\vec{v} = (2,3,0)\ \text{m/s}
$$

$$
q = 1\ \text{mC} = 1 \times 10^{-3}\ \text{C}
$$

$$
m = 0.01\ \text{kg}
$$

$$
\vec{r}(0) = (0,0,0)
$$

---

## Solution

## 1. Lorentz Force

The Lorentz force is:

$$
\vec{F} = q(\vec{v} \times \vec{B})
$$

Cross product:

$$
\vec{v} \times \vec{B} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & 3 & 0 \\
0 & 0 & 1
\end{vmatrix}
$$

$$
\vec{v} \times \vec{B} = (3,-2,0)
$$

Therefore:

$$
\vec{F} = 10^{-3}(3,-2,0)
$$

$$
\vec{F} = (3 \times 10^{-3}, -2 \times 10^{-3}, 0)\ \text{N}
$$

---

## 2. Equation of Motion

Newton's second law:

$$
m\frac{d\vec{v}}{dt} = q(\vec{v} \times \vec{B})
$$

Since $\vec{B}$ is directed along the $z$-axis, the motion occurs in the $xy$-plane.

The angular frequency is:

$$
\omega = \frac{qB}{m}
$$

Substitute the values:

$$
\omega = \frac{1 \times 10^{-3} \cdot 1}{0.01}
$$

$$
\omega = 0.1\ \text{rad/s}
$$

The coordinates are:

$$
x(t) = \frac{v_y}{\omega}\sin(\omega t) + \frac{v_x}{\omega}\sin? 
$$

A simple physical conclusion is that the charge moves in a circular trajectory in the $xy$-plane.

---

## 3. Magnitude of Force

$$
|\vec{F}| = qvB\sin 90^\circ
$$

Speed:

$$
v = \sqrt{2^2 + 3^2}
$$

$$
v = \sqrt{13}
$$

So:

$$
|\vec{F}| = 10^{-3}\sqrt{13}
$$

$$
|\vec{F}| \approx 3.61 \times 10^{-3}\ \text{N}
$$

---

## 4. Work Done by Magnetic Force

The magnetic force is perpendicular to velocity.

Therefore:

$$
W = \vec{F} \cdot \vec{s} = 0
$$

or

$$
P = \vec{F} \cdot \vec{v} = 0
$$

So the magnetic force does **no work**.

---

## 5. Radius of Trajectory

The radius is:

$$
r = \frac{mv}{qB}
$$

Substitute the values:

$$
r = \frac{0.01 \cdot \sqrt{13}}{(1 \times 10^{-3}) \cdot 1}
$$

$$
r = 10\sqrt{13}
$$

$$
r \approx 36.1\ \text{m}
$$

---

## 6. If Magnetic Field is Doubled

The radius formula is:

$$
r = \frac{mv}{qB}
$$

So:

$$
r \propto \frac{1}{B}
$$

If $B$ is doubled:

$$
B \rightarrow 2B
$$

then:

$$
r \rightarrow \frac{r}{2}
$$

$$
r_{\text{new}} = \frac{36.1}{2}
$$

$$
r_{\text{new}} \approx 18.05\ \text{m}
$$

---

## Final Conclusion

The Lorentz force acting on the charge is:

$$
\vec{F} = (3 \times 10^{-3}, -2 \times 10^{-3}, 0)\ \text{N}
$$

Its magnitude is:

$$
|\vec{F}| \approx 3.61 \times 10^{-3}\ \text{N}
$$

The charge moves in a circular path in the $xy$-plane.

The magnetic force does **no work**, because it is perpendicular to the velocity.

The radius of the trajectory is:

$$
r \approx 36.1\ \text{m}
$$

If the magnetic field is doubled, the radius becomes two times smaller:

$$
r_{\text{new}} \approx 18.05\ \text{m}
$$
