# Problem 8 – Two coupled springs (two degrees of freedom)

## Given

Two masses are connected to walls in a series configuration by springs with constants $k_1$, $k_2$, and $k_3$.

We denote:

- $x_1(t)$ — displacement of mass 1
- $x_2(t)$ — displacement of mass 2
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

For the first mass, the forces are:

- spring $k_1$: $-k_1x_1$
- coupling spring $k_2$: $-k_2(x_1 - x_2)$

So,

$$
m_1\ddot{x}_1 = -k_1x_1 - k_2(x_1 - x_2)
$$

Hence,

$$
m_1\ddot{x}_1 + (k_1 + k_2)x_1 - k_2x_2 = 0
$$

For the second mass, the forces are:

- spring $k_3$: $-k_3x_2$
- coupling spring $k_2$: $-k_2(x_2 - x_1)$

So,

$$
m_2\ddot{x}_2 = -k_3x_2 - k_2(x_2 - x_1)
$$

Hence,

$$
m_2\ddot{x}_2 + (k_2 + k_3)x_2 - k_2x_1 = 0
$$

Therefore, the equations of motion are

$$
\boxed{m_1\ddot{x}_1 + (k_1 + k_2)x_1 - k_2x_2 = 0}
$$

$$
\boxed{m_2\ddot{x}_2 + (k_2 + k_3)x_2 - k_2x_1 = 0}
$$

---

### 2. Matrix form

The system can be written as

$$
M\ddot{\mathbf{x}} + K\mathbf{x} = 0
$$

where

$$
\mathbf{x} = \begin{bmatrix} x_1 \\ x_2 \end{bmatrix}
$$

$$
M = \begin{bmatrix} m_1 & 0 \\ 0 & m_2 \end{bmatrix}
$$

$$
K = \begin{bmatrix} k_1 + k_2 & -k_2 \\ -k_2 & k_2 + k_3 \end{bmatrix}
$$

---

### 3. Natural frequencies

Assume harmonic motion:

$$
x_1(t) = A_1e^{i\omega t}, \qquad x_2(t) = A_2e^{i\omega t}
$$

Substitute into the matrix equation:

$$
(K - \omega^2M)\mathbf{A} = 0
$$

For a nonzero solution, the determinant must be zero:

$$
\det(K - \omega^2M) = 0
$$

So,

$$
\begin{vmatrix} k_1 + k_2 - m_1\omega^2 & -k_2 \\ -k_2 & k_2 + k_3 - m_2\omega^2 \end{vmatrix} = 0
$$

Expanding the determinant:

$$
(k_1 + k_2 - m_1\omega^2)(k_2 + k_3 - m_2\omega^2) - k_2^2 = 0
$$

The two roots of this equation give the two natural frequencies:

$$
\boxed{\omega_1,\ \omega_2}
$$

---

### 4. Symmetric case

For the symmetric case,

$$
m_1 = m_2 = m, \qquad k_1 = k_3 = k
$$

the equations become

$$
m\ddot{x}_1 + (k + k_2)x_1 - k_2x_2 = 0
$$

$$
m\ddot{x}_2 + (k + k_2)x_2 - k_2x_1 = 0
$$

Then the determinant equation is

$$
\begin{vmatrix} k + k_2 - m\omega^2 & -k_2 \\ -k_2 & k + k_2 - m\omega^2 \end{vmatrix} = 0
$$

Thus,

$$
(k + k_2 - m\omega^2)^2 - k_2^2 = 0
$$

So,

$$
k + k_2 - m\omega^2 = \pm k_2
$$

From this we get:

For the first mode,

$$
m\omega_1^2 = k
$$

$$
\boxed{\omega_1 = \sqrt{\frac{k}{m}}}
$$

For the second mode,

$$
m\omega_2^2 = k + 2k_2
$$

$$
\boxed{\omega_2 = \sqrt{\frac{k + 2k_2}{m}}}
$$

---

### 5. Normal modes

The normal modes come from solving

$$
(K - \omega^2M)\mathbf{A} = 0
$$

#### First mode

For

$$
\omega_1 = \sqrt{\frac{k}{m}}
$$

the eigenvector is

$$
\boxed{\mathbf{A}_1 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}}
$$

This means both masses move together with the same displacement.

So this is the **in-phase mode**.

#### Second mode

For

$$
\omega_2 = \sqrt{\frac{k + 2k_2}{m}}
$$

the eigenvector is

$$
\boxed{\mathbf{A}_2 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}}
$$

This means the masses move in opposite directions.

So this is the **out-of-phase mode**.

---

### 6. General solution

The general motion is a superposition of the two normal modes:

$$
\mathbf{x}(t) = C_1\mathbf{A}_1\cos(\omega_1 t + \phi_1) + C_2\mathbf{A}_2\cos(\omega_2 t + \phi_2)
$$

For the symmetric case, this becomes

$$
\begin{bmatrix} x_1(t) \\ x_2(t) \end{bmatrix} = C_1\begin{bmatrix} 1 \\ 1 \end{bmatrix}\cos(\omega_1 t + \phi_1) + C_2\begin{bmatrix} 1 \\ -1 \end{bmatrix}\cos(\omega_2 t + \phi_2)
$$

This shows that the total motion is the sum of the in-phase and out-of-phase normal modes.

---

### 7. Numerical solution

Introduce the velocities

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
\dot{v}_1 = \frac{-(k_1 + k_2)x_1 + k_2x_2}{m_1}
$$

$$
\dot{v}_2 = \frac{k_2x_1 - (k_2 + k_3)x_2}{m_2}
$$

So the first-order system is

$$
\boxed{\dot{x}_1 = v_1}
$$

$$
\boxed{\dot{x}_2 = v_2}
$$

$$
\boxed{\dot{v}_1 = \frac{-(k_1 + k_2)x_1 + k_2x_2}{m_1}}
$$

$$
\boxed{\dot{v}_2 = \frac{k_2x_1 - (k_2 + k_3)x_2}{m_2}}
$$

This system can be solved numerically using RK4.

---

### 8. Energy exchange

Because the masses are coupled by the spring $k_2$, energy can pass from one mass to the other.

If initially only one mass is displaced, then:

- first mass starts with most of the energy
- second mass gradually gains energy
- later the first mass loses energy
- then energy flows back again

So the amplitudes of the two masses change with time.

This is the phenomenon of **energy exchange** between coupled oscillators.

---

## Final Answer

The equations of motion are

$$
\boxed{m_1\ddot{x}_1 + (k_1 + k_2)x_1 - k_2x_2 = 0}
$$

$$
\boxed{m_2\ddot{x}_2 + (k_2 + k_3)x_2 - k_2x_1 = 0}
$$

The natural frequencies are found from

$$
\boxed{(k_1 + k_2 - m_1\omega^2)(k_2 + k_3 - m_2\omega^2) - k_2^2 = 0}
$$

For the symmetric case $m_1 = m_2 = m$ and $k_1 = k_3 = k$, the natural frequencies are

$$
\boxed{\omega_1 = \sqrt{\frac{k}{m}}}
$$

$$
\boxed{\omega_2 = \sqrt{\frac{k + 2k_2}{m}}}
$$

The normal modes are

$$
\boxed{\mathbf{A}_1 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}} \qquad \text{in-phase}
$$

$$
\boxed{\mathbf{A}_2 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}} \qquad \text{out-of-phase}
$$

---

## Conclusion

The coupled spring system has two degrees of freedom, so it has two natural frequencies and two normal modes.

- In the first mode, both masses move together.
- In the second mode, they move oppositely.
- For arbitrary initial conditions, the motion is a combination of both modes.
- The coupling spring causes periodic energy exchange between the masses.
