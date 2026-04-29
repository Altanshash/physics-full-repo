# Problem 1 – Lorentz Force

## Given:

- Magnetic field:
  
  $$
  \vec{B} = (0,0,1)\ \text{T}
  $$

- Velocity:
  
  $$
  \vec{v} = (2,3,0)\ \text{m/s}
  $$

- Charge:
  
  $$
  q = 1\,\text{mC} = 1 \times 10^{-3}\ \text{C}
  $$

---

## 1. Lorentz Force

The Lorentz force is given by:

:contentReference[oaicite:0]{index=0}

### Cross product:

$$
\vec{v} \times \vec{B} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & 3 & 0 \\
0 & 0 & 1
\end{vmatrix}
$$

$$
= (3\cdot1 - 0)\hat{i} - (2\cdot1 - 0)\hat{j} + (0 - 0)\hat{k}
$$

$$
= (3, -2, 0)
$$

### Force:

$$
\vec{F} = q (3,-2,0)
$$

$$
\vec{F} = (3\times10^{-3},\ -2\times10^{-3},\ 0)\ \text{N}
$$

---

## 2. Equation of Motion

Newton’s second law:

$$
m \frac{d\vec{v}}{dt} = \vec{F}
$$

Since the force is always perpendicular to velocity, the motion is **circular**.

Trajectory:

$$
x(t), y(t) \rightarrow \text{circular motion in XY plane}
$$

---

## 3. Magnitude of Force

$$
|\vec{F}| = \sqrt{(3\times10^{-3})^2 + (-2\times10^{-3})^2}
$$

$$
= \sqrt{9 + 4} \times 10^{-3}
$$

$$
= \sqrt{13} \times 10^{-3} \approx 3.61 \times 10^{-3}\ \text{N}
$$

---

## 4. Does Magnetic Force Do Work?

Magnetic force is always perpendicular to velocity:

$$
W = \vec{F} \cdot \vec{v} = 0
$$

✅ **Answer:** Magnetic force does **no work**.

---

## 5. Radius of Trajectory

Formula:

$$
r = \frac{mv}{qB}
$$

Speed:

$$
v = \sqrt{2^2 + 3^2} = \sqrt{13}
$$

Now substitute:

$$
r = \frac{0.01 \cdot \sqrt{13}}{(1\times10^{-3}) \cdot 1}
$$

$$
r = 10\sqrt{13} \approx 36.1\ \text{m}
$$

---

## 6. Effect of Doubling Magnetic Field

If $B \rightarrow 2B$, then:

$$
r \propto \frac{1}{B}
$$

So:

$$
r \rightarrow \frac{r}{2}
$$

---

## Final Conclusion

- Lorentz force:
  
  $$
  \vec{F} = (3\times10^{-3}, -2\times10^{-3}, 0)\ \text{N}
  $$

- Magnitude:
  
  $$
  |\vec{F}| \approx 3.61 \times 10^{-3}\ \text{N}
  $$

- Motion: **circular**
- Magnetic force does **no work**
- Radius:
  
  $$
  r \approx 36.1\ \text{m}
  $$

- If magnetic field doubles → radius becomes **2 times smaller**

---
