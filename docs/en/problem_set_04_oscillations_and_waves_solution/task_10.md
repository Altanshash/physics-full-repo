# Problem 10 – Double pendulum and deterministic chaos

## Given

We consider a double pendulum with:

- masses $m_1$, $m_2$
- rod lengths $l_1$, $l_2$
- gravitational acceleration $g$

The starting parameters are

$$
m_1 = m_2 = 1, \qquad l_1 = l_2 = 1, \qquad g = 9.81
$$

We use a numerical integration step

$$
\Delta t \le 0.01\ \text{s}
$$

We need to:

1. Write the coordinates $(x_1,y_1)$ and $(x_2,y_2)$ as functions of the angles $(\theta_1,\theta_2)$.
2. Implement a numerical integration of the equations of motion and check numerical stability.
3. Investigate sensitivity to initial conditions by simulating 50 copies with very small differences.
4. Experiment with different perturbation scales and observe divergence of trajectories.

---

## Solution

### 1. Coordinates of the masses

Let $\theta_1(t)$ be the angle of the first rod and $\theta_2(t)$ the angle of the second rod, measured from the vertical.

Then the coordinates of the first mass are

$$
\boxed{x_1 = l_1 \sin\theta_1}
$$

$$
\boxed{y_1 = -l_1 \cos\theta_1}
$$

The second mass is attached to the end of the first rod, so its coordinates are

$$
\boxed{x_2 = l_1 \sin\theta_1 + l_2 \sin\theta_2}
$$

$$
\boxed{y_2 = -l_1 \cos\theta_1 - l_2 \cos\theta_2}
$$

These formulas are used directly for animation.

---

### 2. Equations of motion

In this problem we do not derive the equations analytically.  
We take the standard equations of motion for the double pendulum in first-order form.

Introduce the angular velocities

$$
\omega_1 = \dot{\theta}_1, \qquad \omega_2 = \dot{\theta}_2
$$

Then the system becomes

$$
\dot{\theta}_1 = \omega_1
$$

$$
\dot{\theta}_2 = \omega_2
$$

and

$$
\dot{\omega}_1 = f_1(\theta_1,\theta_2,\omega_1,\omega_2)
$$

$$
\dot{\omega}_2 = f_2(\theta_1,\theta_2,\omega_1,\omega_2)
$$

For equal masses and general rod lengths, the standard equations are

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

So the full numerical system is

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

### 3. Numerical integration

We solve this system numerically using RK4.

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

Then the system has the form

$$
\dot{\mathbf{y}} = F(\mathbf{y})
$$

The RK4 update is

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

and

$$
\boxed{
\mathbf{y}_{n+1}
=
\mathbf{y}_n
+
\frac{\Delta t}{6}(k_1 + 2k_2 + 2k_3 + k_4)
}
$$

This gives the numerical trajectory of the double pendulum.

---

### 4. Numerical stability

To check numerical stability, we compare the behavior for different time steps:

$$
\Delta t = 0.01,\ 0.005,\ 0.001
$$

A useful criterion is the total mechanical energy.

The kinetic energy is

$$
T =
\frac{1}{2}(m_1+m_2)l_1^2\omega_1^2
+
\frac{1}{2}m_2 l_2^2\omega_2^2
+
m_2 l_1 l_2 \omega_1 \omega_2 \cos(\theta_1-\theta_2)
$$

The potential energy is

$$
V =
-(m_1+m_2)g l_1 \cos\theta_1
-
m_2 g l_2 \cos\theta_2
$$

Therefore the total energy is

$$
\boxed{E = T + V}
$$

If the method is stable and the time step is sufficiently small, the energy drift should remain small over time.

So numerical stability is checked by monitoring:

- whether the trajectories remain physically reasonable
- whether the total energy changes only slightly
- whether smaller $\Delta t$ gives better energy conservation

---

### 5. Sensitivity to initial conditions

The main goal of this problem is to demonstrate deterministic chaos.

We simulate 50 copies of the same system.

All parameters are the same, but the initial value of $\theta_2(0)$ is changed slightly.

For example:

$$
\theta_1^{(j)}(0) = \theta_{1,0}
$$

$$
\theta_2^{(j)}(0) = \theta_{2,0} + j\,\varepsilon
\qquad \text{for } j = 0,1,2,\dots,49
$$

with small perturbation scale

$$
\varepsilon \sim 10^{-4} \text{ to } 10^{-2}
$$

and with the same initial angular velocities:

$$
\omega_1^{(j)}(0) = 0, \qquad \omega_2^{(j)}(0) = 0
$$

At the beginning, all trajectories are almost identical.

After some time, the trajectories separate strongly, even though the initial differences were extremely small.

This is the signature of deterministic chaos.

---

### 6. Divergence of trajectories

To observe divergence, we compare the positions of the pendulums over time.

For two nearby solutions, one can define a separation measure such as

$$
d(t) =
\sqrt{
(\theta_1^{(a)} - \theta_1^{(b)})^2
+
(\theta_2^{(a)} - \theta_2^{(b)})^2
}
$$

Initially, $d(0)$ is very small.

In a chaotic regime, this separation typically grows rapidly with time.

So by changing the perturbation scale $\varepsilon$, we observe:

- for very small perturbation, divergence still appears
- for larger perturbation, divergence appears earlier
- after sufficient time, the trajectories become completely different

Thus the system is highly sensitive to initial conditions.

---

### 7. Interpretation of deterministic chaos

The double pendulum is governed by deterministic equations, so there is no randomness in the model.

However, the long-term evolution is extremely sensitive to the initial state.

This means:

- if the initial conditions differ only by a tiny amount
- then after some time the motions become very different

This is called **deterministic chaos**.

So chaos does not mean “random equations.”  
It means that a deterministic nonlinear system can produce motion that is practically unpredictable over long times.

---

### 8. Practical numerical procedure

A typical numerical experiment is:

1. choose the base initial conditions  
   $$
   \theta_1(0),\ \theta_2(0),\ \omega_1(0),\ \omega_2(0)
   $$

2. create 50 copies with slightly perturbed $\theta_2(0)$

3. integrate all systems simultaneously using RK4

4. compute coordinates using  
   $$
   x_1 = l_1\sin\theta_1,\quad y_1 = -l_1\cos\theta_1
   $$
   $$
   x_2 = l_1\sin\theta_1 + l_2\sin\theta_2,\quad y_2 = -l_1\cos\theta_1 - l_2\cos\theta_2
   $$

5. animate all 50 pendulums with different colors

6. compare the trajectories and observe how they diverge

This directly visualizes chaos.

---

## Final Answer

The coordinates used for animation are

$$
\boxed{x_1 = l_1\sin\theta_1,\qquad y_1 = -l_1\cos\theta_1}
$$

$$
\boxed{x_2 = l_1\sin\theta_1 + l_2\sin\theta_2,\qquad y_2 = -l_1\cos\theta_1 - l_2\cos\theta_2}
$$

The double pendulum is solved numerically in first-order form:

$$
\boxed{\dot{\theta}_1 = \omega_1,\qquad \dot{\theta}_2 = \omega_2}
$$

$$
\boxed{\dot{\omega}_1 = f_1(\theta_1,\theta_2,\omega_1,\omega_2),\qquad \dot{\omega}_2 = f_2(\theta_1,\theta_2,\omega_1,\omega_2)}
$$

The integration is performed using RK4 with

$$
\boxed{\Delta t \le 0.01\ \text{s}}
$$

Numerical stability is checked through energy drift:

$$
\boxed{E = T + V}
$$

To demonstrate deterministic chaos, we simulate 50 copies of the pendulum with slightly different initial values of $\theta_2(0)$.

Even for extremely small perturbations, the trajectories diverge strongly after some time, which demonstrates sensitivity to initial conditions.

---

## Conclusion

The double pendulum is a deterministic but chaotic system.

- Its motion is obtained numerically.
- The coordinates are computed directly from the angles.
- Energy drift is used to test numerical stability.
- Small perturbations in initial conditions produce large differences in trajectories over time.

Therefore, the double pendulum is a classic example of deterministic chaos.
