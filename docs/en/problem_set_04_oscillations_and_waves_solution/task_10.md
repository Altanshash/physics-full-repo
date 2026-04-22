# Problem 10 – Double pendulum and deterministic chaos

## Given

We consider a double pendulum with masses $m_1$ and $m_2$, rod lengths $l_1$ and $l_2$, and gravitational acceleration $g$.

The standard parameters are:

$$
m_1 = m_2 = 1, \qquad l_1 = l_2 = 1, \qquad g = 9.81
$$

The numerical integration step is

$$
\Delta t \le 0.01 \text{ s}
$$

We need to:

1. Write the coordinates $(x_1,y_1)$ and $(x_2,y_2)$ as functions of $(\theta_1,\theta_2)$.
2. Implement numerical integration of the equations of motion.
3. Check numerical stability, for example by monitoring energy drift.
4. Simulate 50 copies of the system with slightly different initial conditions.
5. Investigate how trajectories diverge for different perturbation scales.

---

## Solution

### 1. Coordinates of the masses

Let $\theta_1(t)$ be the angle of the first rod and $\theta_2(t)$ the angle of the second rod.

The coordinates of the first mass are

$$
x_1 = l_1 \sin\theta_1
$$

$$
y_1 = -l_1 \cos\theta_1
$$

The coordinates of the second mass are

$$
x_2 = l_1 \sin\theta_1 + l_2 \sin\theta_2
$$

$$
y_2 = -l_1 \cos\theta_1 - l_2 \cos\theta_2
$$

These formulas are used directly for animation.

---

### 2. First-order numerical system

Introduce the angular velocities

$$
\omega_1 = \dot{\theta}_1, \qquad \omega_2 = \dot{\theta}_2
$$

Then

$$
\dot{\theta}_1 = \omega_1
$$

$$
\dot{\theta}_2 = \omega_2
$$

We use the standard numerical form of the double pendulum equations:

$$
\dot{\omega}_1 =
\frac{
-m_2 l_1 \omega_1^2 \sin(\theta_1-\theta_2)\cos(\theta_1-\theta_2)
+ m_2 g \sin\theta_2 \cos(\theta_1-\theta_2)
- m_2 l_2 \omega_2^2 \sin(\theta_1-\theta_2)
- (m_1+m_2)g\sin\theta_1
}{
l_1\left(m_1 + m_2\sin^2(\theta_1-\theta_2)\right)
}
$$

$$
\dot{\omega}_2 =
\frac{
(m_1+m_2)l_1\omega_1^2\sin(\theta_1-\theta_2)
+ (m_1+m_2)g\sin\theta_1\cos(\theta_1-\theta_2)
+ (m_1+m_2)l_2\omega_2^2\sin(\theta_1-\theta_2)\cos(\theta_1-\theta_2)
- (m_1+m_2)g\sin\theta_2
}{
l_2\left(m_1 + m_2\sin^2(\theta_1-\theta_2)\right)
}
$$

So the full system is

$$
\boxed{\dot{\theta}_1 = \omega_1}
$$

$$
\boxed{\dot{\theta}_2 = \omega_2}
$$

$$
\boxed{\dot{\omega}_1 = f_1(\theta_1,\theta_2,\omega_1,\omega_2)}
$$

$$
\boxed{\dot{\omega}_2 = f_2(\theta_1,\theta_2,\omega_1,\omega_2)}
$$

---

### 3. RK4 numerical integration

Let the state vector be

$$
\mathbf{y}(t) =
\begin{bmatrix}
\theta_1 \\
\theta_2 \\
\omega_1 \\
\omega_2
\end{bmatrix}
$$

Then the system can be written as

$$
\dot{\mathbf{y}} = F(\mathbf{y})
$$

The Runge–Kutta 4th order method is

$$
k_1 = F(\mathbf{y}_n)
$$

$$
k_2 = F\left(\mathbf{y}_n + \frac{\Delta t}{2}k_1\right)
$$

$$
k_3 = F\left(\mathbf{y}_n + \frac{\Delta t}{2}k_2\right)
$$

$$
k_4 = F\left(\mathbf{y}_n + \Delta t\,k_3\right)
$$

and the update formula is

$$
\mathbf{y}_{n+1} = \mathbf{y}_n + \frac{\Delta t}{6}(k_1 + 2k_2 + 2k_3 + k_4)
$$

This method is used for all 50 pendulums simultaneously.

---

### 4. Numerical stability

To check numerical stability, we monitor the total mechanical energy.

The kinetic energy is

$$
T = \frac{1}{2}(m_1+m_2)l_1^2\omega_1^2 + \frac{1}{2}m_2l_2^2\omega_2^2 + m_2l_1l_2\omega_1\omega_2\cos(\theta_1-\theta_2)
$$

The potential energy is

$$
V = -(m_1+m_2)g l_1 \cos\theta_1 - m_2 g l_2 \cos\theta_2
$$

Therefore, the total energy is

$$
E = T + V
$$

If $\Delta t$ is small enough, the energy drift should remain small during the simulation.

So numerical stability is checked by:

1. comparing results for different $\Delta t$
2. observing whether the trajectories remain physically reasonable
3. checking whether the total energy changes only slightly

---

### 5. Sensitivity to initial conditions

To demonstrate deterministic chaos, we simulate 50 copies of the double pendulum.

All parameters are the same, but the initial angle $\theta_2(0)$ is perturbed very slightly.

For the $j$-th pendulum, we take

$$
\theta_1^{(j)}(0) = \theta_{1,0}
$$

$$
\theta_2^{(j)}(0) = \theta_{2,0} + j\varepsilon
$$

for

$$
j = 0,1,2,\dots,49
$$

The initial angular velocities are the same for all copies:

$$
\omega_1^{(j)}(0) = 0, \qquad \omega_2^{(j)}(0) = 0
$$

The perturbation scale is small, for example

$$
\varepsilon \sim 10^{-4} \text{ to } 10^{-2}
$$

At the beginning, all pendulums move almost identically.  
After some time, their trajectories separate strongly.

This is the main signature of deterministic chaos.

---

### 6. Divergence of trajectories

To measure divergence, we can compare two nearby solutions and define

$$
d(t) = \sqrt{(\theta_1^{(a)}-\theta_1^{(b)})^2 + (\theta_2^{(a)}-\theta_2^{(b)})^2}
$$

At the start, $d(0)$ is very small.

As time increases, the separation grows rapidly.

This means:

- very small perturbations produce large differences later
- larger perturbations lead to earlier divergence
- after enough time, the trajectories look completely different

So the double pendulum is extremely sensitive to initial conditions.

---

### 7. Practical numerical procedure

The numerical experiment is:

1. choose base initial conditions  
   $$
   \theta_1(0), \quad \theta_2(0), \quad \omega_1(0), \quad \omega_2(0)
   $$

2. create 50 copies with slightly different values of $\theta_2(0)$

3. integrate all systems simultaneously using RK4

4. compute coordinates using  
   $$
   x_1 = l_1\sin\theta_1, \qquad y_1 = -l_1\cos\theta_1
   $$
   $$
   x_2 = l_1\sin\theta_1 + l_2\sin\theta_2, \qquad y_2 = -l_1\cos\theta_1 - l_2\cos\theta_2
   $$

5. animate all 50 pendulums with different colors

6. compare the trajectories and observe how they diverge

This directly visualizes deterministic chaos.

---

## Final Answer

The coordinates for animation are

$$
\boxed{x_1 = l_1\sin\theta_1, \qquad y_1 = -l_1\cos\theta_1}
$$

$$
\boxed{x_2 = l_1\sin\theta_1 + l_2\sin\theta_2, \qquad y_2 = -l_1\cos\theta_1 - l_2\cos\theta_2}
$$

The double pendulum is solved numerically in first-order form:

$$
\boxed{\dot{\theta}_1 = \omega_1, \qquad \dot{\theta}_2 = \omega_2}
$$

$$
\boxed{\dot{\omega}_1 = f_1(\theta_1,\theta_2,\omega_1,\omega_2), \qquad \dot{\omega}_2 = f_2(\theta_1,\theta_2,\omega_1,\omega_2)}
$$

The RK4 method is used with

$$
\boxed{\Delta t \le 0.01 \text{ s}}
$$

The total energy is

$$
\boxed{E = T + V}
$$

where

$$
T = \frac{1}{2}(m_1+m_2)l_1^2\omega_1^2 + \frac{1}{2}m_2l_2^2\omega_2^2 + m_2l_1l_2\omega_1\omega_2\cos(\theta_1-\theta_2)
$$

and

$$
V = -(m_1+m_2)g l_1 \cos\theta_1 - m_2 g l_2 \cos\theta_2
$$

To show chaos, we simulate 50 pendulums with slightly different initial values of $\theta_2(0)$.

Even tiny perturbations lead to large differences in trajectories after some time.

---

## Conclusion

The double pendulum is a deterministic nonlinear system, but it shows chaotic behavior.

- The motion is computed numerically.
- The coordinates are obtained directly from the angles.
- Stability is checked through energy drift.
- Tiny differences in initial conditions grow strongly with time.

Therefore, the double pendulum is a classical example of deterministic chaos.
