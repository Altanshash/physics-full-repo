# Problem 10 – Double pendulum and deterministic chaos

## Given

We consider a double pendulum with masses $m_1$ and $m_2$, rod lengths $l_1$ and $l_2$, and gravitational acceleration $g$.

Standard parameters:

$$
m_1 = m_2 = 1, \qquad l_1 = l_2 = 1, \qquad g = 9.81
$$

Numerical integration step:

$$
\Delta t \le 0.01 \text{ s}
$$

We need to:

1. Write the coordinates $(x_1,y_1)$ and $(x_2,y_2)$ as functions of $(\theta_1,\theta_2)$.
2. Implement numerical integration of the equations of motion.
3. Check numerical stability using energy drift.
4. Simulate 50 copies of the system with slightly different initial conditions.
5. Investigate divergence for different perturbation scales.

---

## Solution

### 1. Coordinates of the masses

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

These formulas are used for visualization and animation.

---

### 2. First-order numerical system

Introduce angular velocities

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

We use the standard double pendulum equations in numerical form.

For $\omega_1$:

$$
\dot{\omega}_1 = \frac{-m_2 l_1 \omega_1^2 \sin(\theta_1-\theta_2)\cos(\theta_1-\theta_2) + m_2 g \sin\theta_2 \cos(\theta_1-\theta_2) - m_2 l_2 \omega_2^2 \sin(\theta_1-\theta_2) - (m_1+m_2)g\sin\theta_1}{l_1\left(m_1 + m_2\sin^2(\theta_1-\theta_2)\right)}
$$

For $\omega_2$:

$$
\dot{\omega}_2 = \frac{(m_1+m_2)l_1\omega_1^2\sin(\theta_1-\theta_2) + (m_1+m_2)g\sin\theta_1\cos(\theta_1-\theta_2) + (m_1+m_2)l_2\omega_2^2\sin(\theta_1-\theta_2)\cos(\theta_1-\theta_2) - (m_1+m_2)g\sin\theta_2}{l_2\left(m_1 + m_2\sin^2(\theta_1-\theta_2)\right)}
$$

So the numerical system is

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
\mathbf{y}(t) = \begin{bmatrix} \theta_1 \\ \theta_2 \\ \omega_1 \\ \omega_2 \end{bmatrix}
$$

Then the system is

$$
\dot{\mathbf{y}} = F(\mathbf{y})
$$

The RK4 method is

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

and the update rule is

$$
\mathbf{y}_{n+1} = \mathbf{y}_n + \frac{\Delta t}{6}(k_1 + 2k_2 + 2k_3 + k_4)
$$

This method is applied to all 50 systems.

---

### 4. Numerical stability

We check numerical stability by monitoring the total mechanical energy.

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

A stable numerical method should show only small energy drift when $\Delta t$ is sufficiently small.

So we compare results for different time steps, for example:

$$
\Delta t = 0.01, \qquad \Delta t = 0.005, \qquad \Delta t = 0.001
$$

Smaller $\Delta t$ should improve energy conservation.

---

### 5. Sensitivity to initial conditions

To demonstrate deterministic chaos, we simulate 50 copies of the pendulum.

All parameters are the same, but $\theta_2(0)$ is slightly perturbed.

For pendulum number $j$, we use

$$
\theta_1^{(j)}(0) = \theta_{1,0}
$$

$$
\theta_2^{(j)}(0) = \theta_{2,0} + j\varepsilon
$$

where

$$
j = 0,1,2,\dots,49
$$

The initial angular velocities are

$$
\omega_1^{(j)}(0) = 0, \qquad \omega_2^{(j)}(0) = 0
$$

The perturbation scale is small, for example

$$
\varepsilon \sim 10^{-4} \text{ to } 10^{-2}
$$

At first, all trajectories are almost identical.  
Later, they separate strongly.

This shows sensitivity to initial conditions.

---

### 6. Divergence of trajectories

To quantify divergence, we can define the distance between two nearby trajectories:

$$
d(t) = \sqrt{(\theta_1^{(a)}-\theta_1^{(b)})^2 + (\theta_2^{(a)}-\theta_2^{(b)})^2}
$$

At the beginning, $d(t)$ is very small.

As time grows, the separation increases rapidly.

This means:

1. tiny initial differences produce large later differences
2. larger perturbations lead to earlier divergence
3. long-term motion becomes practically unpredictable

This is the main property of deterministic chaos.

---

### 7. Practical numerical procedure

The numerical experiment is performed as follows:

1. choose base initial conditions  
   $$
   \theta_1(0), \quad \theta_2(0), \quad \omega_1(0), \quad \omega_2(0)
   $$

2. create 50 copies with slightly different $\theta_2(0)$

3. integrate all systems simultaneously using RK4

4. compute coordinates using  
   $$
   x_1 = l_1\sin\theta_1, \qquad y_1 = -l_1\cos\theta_1
   $$
   $$
   x_2 = l_1\sin\theta_1 + l_2\sin\theta_2, \qquad y_2 = -l_1\cos\theta_1 - l_2\cos\theta_2
   $$

5. animate all 50 pendulums in different colors

6. observe how initially close trajectories diverge

This directly visualizes deterministic chaos.

---

## Final Answer

The coordinates are

$$
\boxed{x_1 = l_1\sin\theta_1, \qquad y_1 = -l_1\cos\theta_1}
$$

$$
\boxed{x_2 = l_1\sin\theta_1 + l_2\sin\theta_2, \qquad y_2 = -l_1\cos\theta_1 - l_2\cos\theta_2}
$$

The first-order numerical system is

$$
\boxed{\dot{\theta}_1 = \omega_1, \qquad \dot{\theta}_2 = \omega_2}
$$

$$
\boxed{\dot{\omega}_1 = f_1(\theta_1,\theta_2,\omega_1,\omega_2), \qquad \dot{\omega}_2 = f_2(\theta_1,\theta_2,\omega_1,\omega_2)}
$$

The total energy is

$$
\boxed{E = T + V}
$$

with

$$
T = \frac{1}{2}(m_1+m_2)l_1^2\omega_1^2 + \frac{1}{2}m_2l_2^2\omega_2^2 + m_2l_1l_2\omega_1\omega_2\cos(\theta_1-\theta_2)
$$

and

$$
V = -(m_1+m_2)g l_1 \cos\theta_1 - m_2 g l_2 \cos\theta_2
$$

To show chaos, 50 pendulums are simulated with slightly different initial values of $\theta_2(0)$.

Even extremely small perturbations lead to strong divergence of trajectories.

---

## Conclusion

The double pendulum is a deterministic nonlinear system that exhibits chaos.

- The motion is obtained numerically.
- The coordinates are computed directly from the angles.
- Numerical stability is checked using energy drift.
- Tiny differences in initial conditions grow rapidly with time.

Therefore, the double pendulum is a classical example of deterministic chaos.
