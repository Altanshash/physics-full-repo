# Problem 9 – Chain of $N$ springs (discrete wave model)

## Given

System: $N$ masses connected by springs.

We denote:

- $u_n(t)$ — displacement of the $n$-th mass
- $m$ — mass of each particle
- $k$ — spring constant
- $n = 1,2,\dots,N$

We need to:

1. Write down the equations of motion.
2. Solve numerically for $N = 20, 50, 100$.
3. Introduce a local initial disturbance.
4. Observe the propagation of the pulse.
5. Investigate the effect of the values of $k$ and $m$ on the propagation speed.

---

## Solution

### 1. Equations of motion

Consider a chain of identical masses connected by identical springs.

For an interior mass $n$, the force from the left spring is proportional to $u_{n-1} - u_n$, and the force from the right spring is proportional to $u_{n+1} - u_n$.

So the total force is

$$
F_n = k(u_{n+1} - u_n) - k(u_n - u_{n-1})
$$

Simplify:

$$
F_n = k(u_{n+1} - 2u_n + u_{n-1})
$$

Using Newton's second law,

$$
m\ddot{u}_n = F_n
$$

therefore,

$$
\boxed{m\ddot{u}_n = k(u_{n+1} - 2u_n + u_{n-1})}
$$

for $n = 2,3,\dots,N-1$.

This is the discrete wave equation for the chain.

---

### 2. Boundary conditions

The exact form depends on the ends of the chain.

#### Fixed ends

If both ends are fixed, then

$$
u_0 = 0, \qquad u_{N+1} = 0
$$

and for the first and last masses:

$$
m\ddot{u}_1 = k(u_2 - 2u_1)
$$

$$
m\ddot{u}_N = k(u_{N-1} - 2u_N)
$$

#### Free ends

If the ends are free, then different boundary conditions are used.

In this problem, the simplest choice is to use **fixed ends**.

---

### 3. Matrix form

Let

$$
\mathbf{u}(t) =
\begin{bmatrix}
u_1(t) \\
u_2(t) \\
\vdots \\
u_N(t)
\end{bmatrix}
$$

Then the system can be written as

$$
m\ddot{\mathbf{u}} = K\mathbf{u}
$$

where the tridiagonal matrix is

$$
K = k
\begin{bmatrix}
-2 & 1 & 0 & \cdots & 0 \\
1 & -2 & 1 & \cdots & 0 \\
0 & 1 & -2 & \cdots & 0 \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
0 & 0 & 0 & 1 & -2
\end{bmatrix}
$$

So the full system is a coupled system of $N$ second-order differential equations.

---

### 4. Numerical solution

To solve numerically, introduce the velocity of each mass:

$$
v_n = \dot{u}_n
$$

Then

$$
\dot{u}_n = v_n
$$

and

$$
\dot{v}_n = \frac{k}{m}(u_{n+1} - 2u_n + u_{n-1})
$$

Thus the first-order system is

$$
\boxed{\dot{u}_n = v_n}
$$

$$
\boxed{\dot{v}_n = \frac{k}{m}(u_{n+1} - 2u_n + u_{n-1})}
$$

for all interior masses.

This system can be solved numerically using RK4 or another time-stepping method.

We perform the computation for

$$
N = 20,\qquad N = 50,\qquad N = 100
$$

to compare the behavior for different chain lengths.

---

### 5. Local initial disturbance

To generate a pulse, we choose a local initial displacement.

For example, we can take

$$
u_n(0) =
\begin{cases}
A, & n = n_0 \\
0, & n \ne n_0
\end{cases}
$$

with all initial velocities equal to zero:

$$
v_n(0) = 0
$$

This means that initially only one mass is displaced.

Another common choice is a Gaussian pulse:

$$
u_n(0) = A\exp\left(-\frac{(n-n_0)^2}{\sigma^2}\right)
$$

$$
v_n(0) = 0
$$

This produces a smoother disturbance.

---

### 6. Propagation of the pulse

After the local disturbance is introduced, the displacement spreads through the chain.

What we observe:

1. the initial pulse splits and propagates along the chain
2. neighboring masses begin to oscillate
3. the disturbance travels from one mass to the next
4. reflections appear when the pulse reaches the boundaries
5. the pulse gradually spreads because the system is discrete

So the chain behaves like a discrete model of wave propagation.

---

### 7. Effect of $N$

The value of $N$ changes how the chain looks and how finely the wave is represented.

- For $N = 20$, the chain is short and coarse.
- For $N = 50$, the pulse propagation looks smoother.
- For $N = 100$, the chain behaves more like a continuous medium.

As $N$ increases, the discrete model better approximates a continuous string or elastic medium.

---

### 8. Effect of $k$ and $m$ on propagation speed

From the discrete equation

$$
m\ddot{u}_n = k(u_{n+1} - 2u_n + u_{n-1})
$$

we see that the motion depends on the ratio

$$
\frac{k}{m}
$$

If $k$ increases:

- the springs become stiffer
- the interaction between neighboring masses becomes stronger
- the disturbance propagates faster

If $m$ increases:

- the masses become heavier
- acceleration becomes smaller
- the disturbance propagates more slowly

So the propagation speed increases with larger $k$ and decreases with larger $m$.

In qualitative form:

$$
\boxed{c \propto \sqrt{\frac{k}{m}}}
$$

Thus the speed depends on the square root of the stiffness-to-mass ratio.

---

### 9. Physical interpretation

This system is a discrete model of a wave medium.

- Each mass interacts only with its nearest neighbors.
- A local displacement creates a disturbance.
- That disturbance propagates through the chain as a wave.
- Energy is transferred from one mass to the next by the springs.

So the chain of springs is a simple physical model for wave propagation in lattices and solids.

---

## Final Answer

The equations of motion for the chain are

$$
\boxed{m\ddot{u}_n = k(u_{n+1} - 2u_n + u_{n-1})}
$$

for interior masses.

With velocities introduced, the numerical first-order system is

$$
\boxed{\dot{u}_n = v_n}
$$

$$
\boxed{\dot{v}_n = \frac{k}{m}(u_{n+1} - 2u_n + u_{n-1})}
$$

A local disturbance can be introduced by choosing, for example,

$$
\boxed{
u_n(0) =
\begin{cases}
A, & n = n_0 \\
0, & n \ne n_0
\end{cases}
}
$$

with

$$
\boxed{v_n(0) = 0}
$$

The pulse then propagates along the chain, reflects at the boundaries, and spreads because the system is discrete.

The propagation speed depends on $k$ and $m$ approximately as

$$
\boxed{c \propto \sqrt{\frac{k}{m}}}
$$

---

## Conclusion

A chain of $N$ coupled masses and springs is a discrete wave model.

- The equations of motion form a system of coupled differential equations.
- A local initial disturbance propagates through the chain like a wave.
- Larger $k$ gives faster propagation.
- Larger $m$ gives slower propagation.
- Increasing $N$ makes the chain behave more like a continuous medium.

This model clearly shows how wave motion can arise from local interactions between neighboring masses.
