# Problem 8 – Two coupled springs (two degrees of freedom)

## Given

Two masses are connected to walls in a series configuration by springs with constants $k_1$, $k_2$, and $k_3$.

We denote:

- $x_1(t)$ — displacement of the first mass
- $x_2(t)$ — displacement of the second mass
- $m_1$, $m_2$ — the masses

We need to:

1. Write down the equations of motion.
2. Determine the natural frequencies.
3. Find the normal modes.
4. Solve numerically for arbitrary initial conditions.
5. Identify the energy exchange between the masses.

---

## Solution

### 1. Equations of motion

Let $x_1$ and $x_2$ be small displacements from equilibrium.

#### Forces acting on mass $m_1$

- The spring $k_1$ gives force $-k_1 x_1$
- The coupling spring $k_2$ depends on the relative displacement, so its force is $-k_2(x_1 - x_2)$

Therefore, for mass $m_1$:

$$
m_1 \ddot{x}_1 = -k_1 x_1 - k_2(x_1 - x_2)
$$

Simplify:

$$
m_1 \ddot{x}_1 = -(k_1 + k_2)x_1 + k_2 x_2
$$

So,

$$
\boxed{
m_1 \ddot{x}_1 + (k_1 + k_2)x_1 - k_2 x_2 = 0
}
$$

---

#### Forces acting on mass $m_2$

- The spring $k_3$ gives force $-k_3 x_2$
- The coupling spring $k_2$ gives force $-k_2(x_2 - x_1)$

Therefore, for mass $m_2$:

$$
m_2 \ddot{x}_2 = -k_3 x_2 - k_2(x_2 - x_1)
$$

Simplify:

$$
m_2 \ddot{x}_2 = k_2 x_1 - (k_2 + k_3)x_2
$$

So,

$$
\boxed{
m_2 \ddot{x}_2 + (k_2 + k_3)x_2 - k_2 x_1 = 0
}
$$

---

### 2. Matrix form

The system can be written as

$$
\boxed{
M \ddot{\mathbf{x}} + K \mathbf{x} = 0
}
$$

where

$$
\mathbf{x} =
\begin{bmatrix}
x_1 \\
x_2
\end{bmatrix}
$$

$$
M =
\begin{bmatrix}
m_1 & 0 \\
0 & m_2
\end{bmatrix}
$$

$$
K =
\begin{bmatrix}
k_1 + k_2 & -k_2 \\
-k_2 & k_2 + k_3
\end{bmatrix}
$$

---

### 3. Natural frequencies

To find the natural frequencies, assume harmonic motion:

$$
x_1(t) = A_1 e^{i\omega t}, \qquad x_2(t) = A_2 e^{i\omega t}
$$

Substitute into the matrix equation:

$$
(-\omega^2 M + K)\mathbf{A} = 0
$$

For a nontrivial solution, the determinant must vanish:

$$
\boxed{
\det(K - \omega^2 M) = 0
}
$$

That is,

$$
\begin{vmatrix}
k_1 + k_2 - m_1\omega^2 & -k_2 \\
-k_2 & k_2 + k_3 - m_2\omega^2
\end{vmatrix}
= 0
$$

Expanding the determinant:

$$
(k_1 + k_2 - m_1\omega^2)(k_2 + k_3 - m_2\omega^2) - k_2^2 = 0
$$

This is the characteristic equation for $\omega^2$.

Therefore, the two roots give the two natural frequencies:

$$
\boxed{\omega_1,\ \omega_2}
$$

with $\omega_1 < \omega_2$.

---

### 4. Special symmetric case

If

$$
m_1 = m_2 = m, \qquad k_1 = k_3 = k
$$

then the equations become

$$
m\ddot{x}_1 + (k + k_2)x_1 - k_2 x_2 = 0
$$

$$
m\ddot{x}_2 + (k + k_2)x_2 - k_2 x_1 = 0
$$

The determinant equation becomes

$$
\begin{vmatrix}
k + k_2 - m\omega^2 & -k_2 \\
-k_2 & k + k_2 - m\omega^2
\end{vmatrix}
= 0
$$

So

$$
(k + k_2 - m\omega^2)^2 - k_2^2 = 0
$$

This gives

$$
k + k_2 - m\omega^2 = \pm k_2
$$

Hence the two natural frequencies are

$$
\boxed{
\omega_1 = \sqrt{\frac{k}{m}}
}
$$

and

$$
\boxed{
\omega_2 = \sqrt{\frac{k + 2k_2}{m}}
}
$$

---

### 5. Normal modes

The normal modes are obtained from

$$
(K - \omega^2 M)\mathbf{A} = 0
$$

#### First mode: lower frequency mode

For

$$
\omega_1 = \sqrt{\frac{k}{m}}
$$

the eigenvector is

$$
\boxed{
\mathbf{A}_1 =
\begin{bmatrix}
1 \\
1
\end{bmatrix}
}
$$

This means both masses move in the same direction with the same amplitude.

So the first mode is the **in-phase mode**.

---

#### Second mode: higher frequency mode

For

$$
\omega_2 = \sqrt{\frac{k + 2k_2}{m}}
$$

the eigenvector is

$$
\boxed{
\mathbf{A}_2 =
\begin{bmatrix}
1 \\
-1
\end{bmatrix}
}
$$

This means the two masses move in opposite directions.

So the second mode is the **out-of-phase mode**.

---

### 6. General solution

The general motion is a superposition of the two normal modes:

$$
\mathbf{x}(t) = C_1 \mathbf{A}_1 \cos(\omega_1 t + \phi_1) + C_2 \mathbf{A}_2 \cos(\omega_2 t + \phi_2)
$$

For the symmetric case, this can be written as

$$
\begin{bmatrix}
x_1(t) \\
x_2(t)
\end{bmatrix}
=
C_1
\begin{bmatrix}
1 \\
1
\end{bmatrix}
\cos(\omega_1 t + \phi_1)
+
C_2
\begin{bmatrix}
1 \\
-1
\end{bmatrix}
\cos(\omega_2 t + \phi_2)
$$

This shows that the motion is the sum of the in-phase and out-of-phase modes.

---

### 7. Numerical solution

To solve numerically, introduce velocities:

$$
v_1 = \dot{x}_1, \qquad v_2 = \dot{x}_2
$$

Then the system becomes

$$
\dot{x}_1 = v_1
$$

$$
\dot{x}_2 = v_2
$$

$$
\dot{v}_1 = \frac{-(k_1 + k_2)x_1 + k_2 x_2}{m_1}
$$

$$
\dot{v}_2 = \frac{k_2 x_1 - (k_2 + k_3)x_2}{m_2}
$$

So the numerical system is

$$
\boxed{
\dot{x}_1 = v_1
}
$$

$$
\boxed{
\dot{x}_2 = v_2
}
$$

$$
\boxed{
\dot{v}_1 = \frac{-(k_1 + k_2)x_1 + k_2 x_2}{m_1}
}
$$

$$
\boxed{
\dot{v}_2 = \frac{k_2 x_1 - (k_2 + k_3)x_2}{m_2}
}
$$

This system can be solved using RK4 for arbitrary initial conditions.

---

### 8. Energy exchange

The total mechanical energy is exchanged between the two masses through the coupling spring $k_2$.

If only one mass is initially displaced, then:

- the first mass starts moving first
- the second mass gradually begins to oscillate
- later the first mass loses energy while the second gains energy
- then the energy flows back again

This produces the phenomenon of **energy exchange** or **beats** between the two oscillators.

So:

- when one mass has large amplitude, the other often has smaller amplitude
- after some time, the situation reverses

This is a characteristic feature of coupled oscillators.

---

## Final Answer

The equations of motion are

$$
\boxed{
m_1 \ddot{x}_1 + (k_1 + k_2)x_1 - k_2 x_2 = 0
}
$$

$$
\boxed{
m_2 \ddot{x}_2 + (k_2 + k_3)x_2 - k_2 x_1 = 0
}
$$

The natural frequencies are obtained from

$$
\boxed{
\det(K - \omega^2 M) = 0
}
$$

that is,

$$
\boxed{
(k_1 + k_2 - m_1\omega^2)(k_2 + k_3 - m_2\omega^2) - k_2^2 = 0
}
$$

For the symmetric case $m_1 = m_2 = m$ and $k_1 = k_3 = k$, the natural frequencies are

$$
\boxed{
\omega_1 = \sqrt{\frac{k}{m}}
}
$$

$$
\boxed{
\omega_2 = \sqrt{\frac{k + 2k_2}{m}}
}
$$

The normal modes are

$$
\boxed{
\mathbf{A}_1 =
\begin{bmatrix}
1 \\
1
\end{bmatrix}
}
\quad \text{(in-phase)}
$$

$$
\boxed{
\mathbf{A}_2 =
\begin{bmatrix}
1 \\
-1
\end{bmatrix}
}
\quad \text{(out-of-phase)}
$$

---

## Conclusion

The coupled spring system has two degrees of freedom, so it has two natural frequencies and two normal modes.

- In the first mode, both masses move together.
- In the second mode, they move oppositely.
- For arbitrary initial conditions, the motion is a combination of both modes.
- Because of the coupling spring, energy is transferred back and forth between the two masses.

This energy exchange is one of the main physical features of coupled oscillators.
