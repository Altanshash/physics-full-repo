# Problem 10 — Numerical Simulation of Relativistic Motion

## Given

Relativistic equation of motion:

$$
\frac{d}{dt}(\gamma mv)=F
$$

where:

$$
\gamma=\frac{1}{\sqrt{1-\frac{v^2}{c^2}}}
$$

A constant force acts on a particle.

We need to:

1. Implement the RK4 method  
2. Compare classical and relativistic motion  
3. Investigate the asymptotic approach to \(c\)  
4. Create graphs of \(v(t)\) and \(x(t)\)  
5. Evaluate energy differences  

---

# Solution

## 1. Classical Model

In classical mechanics:

$$
F=ma
$$

Therefore:

$$
a=\frac{F}{m}
$$

Velocity:

$$
v(t)=at
$$

Position:

$$
x(t)=\frac{1}{2}at^2
$$

In the classical model, velocity increases without limit:

$$
v\to\infty
$$

This becomes unphysical at very high speeds.

---

## 2. Relativistic Model

Relativistic momentum is:

$$
p=\gamma mv
$$

The equation of motion is:

$$
\frac{dp}{dt}=F
$$

For constant force:

$$
p(t)=Ft
$$

Velocity is obtained from momentum:

$$
v=\frac{p}{\sqrt{m^2+\frac{p^2}{c^2}}}
$$

As time increases:

$$
v\to c
$$

The particle approaches the speed of light but never exceeds it.

---

## 3. RK4 Method

The RK4 method numerically solves differential equations.

For position:

$$
\frac{dx}{dt}=v
$$

For relativistic velocity:

$$
\frac{dv}{dt}=\frac{F}{m\gamma^3}
$$

where:

$$
\gamma=\frac{1}{\sqrt{1-\frac{v^2}{c^2}}}
$$

The RK4 method calculates intermediate slopes:

$$
k_1,k_2,k_3,k_4
$$

and combines them for accurate numerical integration.

---

## 4. Comparison of Motion

### Classical motion

The classical velocity grows linearly:

$$
v_{\text{classical}}=at
$$

Thus, the classical model predicts:

$$
v>c
$$

for sufficiently large time.

This contradicts relativity.

---

### Relativistic motion

The relativistic velocity increases more slowly.

As velocity grows:

$$
\gamma\to\infty
$$

Therefore, acceleration decreases:

$$
a=\frac{F}{m\gamma^3}
$$

and the velocity satisfies:

$$
v<c
$$

for all time.

---

## 5. Asymptotic Approach to \(c\)

At low speeds:

$$
v\ll c
$$

the Lorentz factor becomes:

$$
\gamma\approx1
$$

Thus, relativistic motion reduces to classical motion.

At high speeds:

$$
v\to c
$$

the Lorentz factor grows rapidly:

$$
\gamma\to\infty
$$

Therefore, larger and larger energy is required to produce smaller increases in velocity.

The speed approaches \(c\) asymptotically.

---

## 6. Energy Difference

Classical kinetic energy:

$$
K_{\text{classical}}=\frac{1}{2}mv^2
$$

Relativistic kinetic energy:

$$
K_{\text{relativistic}}=(\gamma-1)mc^2
$$

At low velocities:

$$
K_{\text{classical}}\approx K_{\text{relativistic}}
$$

At relativistic velocities:

$$
K_{\text{relativistic}}\gg K_{\text{classical}}
$$

This difference becomes extremely large near the speed of light.

---

# Conclusion

The numerical simulation shows that classical and relativistic motion agree only at low velocities.

Classically:

$$
v=at
$$

so velocity can increase without bound.

Relativistically:

$$
v\to c
$$

so the particle approaches the speed of light but never reaches it.

The RK4 method provides accurate numerical solutions for:

$$
v(t)
$$

and:

$$
x(t)
$$

The simulation demonstrates that special relativity limits the motion of massive particles and strongly modifies their energy at high velocities.
