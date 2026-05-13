# Problem 10 – Stability Analysis and Conserved Quantities

## Given

For the three-body system, we monitor the following quantities:

1. Total energy:

$$E(t)$$

2. Angular momentum:

$$L=r\times mv$$

3. Position of the center of mass.

The goal is to evaluate the stability of the numerical method, compare different time steps, and investigate the effect of the integration scheme.

---

## Solution

### 1. Total Energy

The total energy of the three-body system is the sum of kinetic and potential energy.

The kinetic energy is:

$$K=\sum_i \frac{1}{2}m_i v_i^2$$

The gravitational potential energy is:

$$U=-\sum_{i<j}\frac{Gm_im_j}{r_{ij}}$$

Therefore, the total energy is:

$$E=K+U$$

For an ideal isolated system, total energy must remain constant:

$$E(t)=constant$$

---

### 2. Angular Momentum

The angular momentum of one body is:

$$L_i=r_i\times m_i v_i$$

The total angular momentum is:

$$L=\sum_i L_i$$

For an isolated system:

$$L(t)=constant$$

If angular momentum changes significantly, the numerical method is unstable or inaccurate.

---

### 3. Center of Mass

The center of mass is:

$$R=\frac{\sum_i m_i r_i}{\sum_i m_i}$$

For an isolated system, the center of mass should remain fixed or move with constant velocity.

If the initial total momentum is zero, then the center of mass should stay near the same point.

---

### 4. Stability of the Numerical Method

The stability of the numerical method is evaluated by checking whether conserved quantities remain nearly constant.

A stable numerical method should keep:

$$E(t)\approx E(0)$$

$$L(t)\approx L(0)$$

and the center of mass should not drift significantly.

---

### 5. Effect of Time Step

The time step is denoted by:

$$\Delta t$$

If the time step is small, the simulation is usually more accurate.

If the time step is large, numerical errors grow faster.

Therefore:

- Small $\Delta t$ gives better conservation.
- Large $\Delta t$ gives faster simulation but lower accuracy.
- Very large $\Delta t$ may make the system unstable.

---

### 6. Effect of Integration Scheme

Different integration schemes give different accuracy.

Euler method is simple but less stable.

RK4 method is more accurate and usually conserves energy and angular momentum better for short simulations.

However, for long-term orbital simulations, symplectic methods are often more stable.

---

## HTML Requirements

The HTML visualization should include:

- graph of total energy $E(t)$
- graph of angular momentum $L(t)$
- graph or marker of the center of mass
- time step slider $\Delta t$
- integration scheme comparison

---

## Conclusion

For a three-body system, the motion can be chaotic, but important physical quantities should remain conserved in an isolated system.

The main conserved quantities are:

$$E(t)$$

$$L(t)$$

and the motion of the center of mass.

A good numerical method keeps these values nearly constant.

By comparing different time steps $\Delta t$, we can see that smaller time steps improve numerical stability, while larger time steps increase numerical error.

Thus, stability analysis helps determine whether the simulation is physically reliable.
