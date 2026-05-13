# Problem 9 – Three-body System

## Given

We consider three bodies with masses:

- $m_1$
- $m_2$
- $m_3$

Their position vectors are:

- $r_1$
- $r_2$
- $r_3$

The goal is to write the equations of motion, implement a numerical method, and investigate the stability of the system.

---

## Solution

### 1. Equations of Motion

Each body is attracted by the other two bodies.

For body 1:

$$m_1\ddot{r}_1=Gm_1m_2\frac{r_2-r_1}{|r_2-r_1|^3}+Gm_1m_3\frac{r_3-r_1}{|r_3-r_1|^3}$$

For body 2:

$$m_2\ddot{r}_2=Gm_2m_1\frac{r_1-r_2}{|r_1-r_2|^3}+Gm_2m_3\frac{r_3-r_2}{|r_3-r_2|^3}$$

For body 3:

$$m_3\ddot{r}_3=Gm_3m_1\frac{r_1-r_3}{|r_1-r_3|^3}+Gm_3m_2\frac{r_2-r_3}{|r_2-r_3|^3}$$

After dividing by mass:

$$\ddot{r}_1=Gm_2\frac{r_2-r_1}{|r_2-r_1|^3}+Gm_3\frac{r_3-r_1}{|r_3-r_1|^3}$$

$$\ddot{r}_2=Gm_1\frac{r_1-r_2}{|r_1-r_2|^3}+Gm_3\frac{r_3-r_2}{|r_3-r_2|^3}$$

$$\ddot{r}_3=Gm_1\frac{r_1-r_3}{|r_1-r_3|^3}+Gm_2\frac{r_2-r_3}{|r_2-r_3|^3}$$

---

### 2. Numerical Method

A numerical method such as RK4 can be used to update the positions and velocities.

The state of each body is:

$$r_i=(x_i,y_i)$$

$$v_i=(v_{xi},v_{yi})$$

The system is updated using:

$$\frac{dr_i}{dt}=v_i$$

$$\frac{dv_i}{dt}=a_i$$

where $a_i$ is the gravitational acceleration caused by the other two bodies.

---

### 3. Stability of the Configuration

The three-body problem is generally unstable.

Small changes in initial positions, velocities, or masses can produce very different trajectories.

Stable motion is possible only for special configurations, such as:

- symmetric configurations
- nearly circular hierarchical systems
- special periodic orbits

In most cases, the motion becomes chaotic.

---

## HTML Requirements

The HTML visualization should include:

- animation of three-body motion
- ability to change masses
- ability to change initial conditions

---

## Conclusion

The three-body system is more complex than the two-body system.

Each body is affected by the gravitational forces of the other two bodies.

The equations of motion are nonlinear and usually cannot be solved exactly.

A numerical method such as RK4 is used to simulate the motion.

The system is often chaotic, meaning that small changes in initial conditions can lead to large differences in the final motion.
