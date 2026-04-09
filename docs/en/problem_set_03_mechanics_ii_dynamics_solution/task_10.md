## Problem 10 – Numerical model of a dynamical system

### Problem statement

Consider motion in the one-dimensional potential

$$
U(x) = \frac{k}{2}x^2 + \lambda x^4
$$

Determine:

- the force,
- the equation of motion,
- a numerical solution for selected parameters,
- the effect of the initial energy on the type of motion,
- a visualization of $x(t)$ and the phase portrait.

---

## Solution

### 1. Force

The force is the negative derivative of the potential:

$$
F(x) = -\frac{dU}{dx}
$$

Differentiate:

$$
\frac{dU}{dx} = kx + 4\lambda x^3
$$

Therefore,

$$
\boxed{
F(x) = -kx - 4\lambda x^3
}
$$

---

### 2. Equation of motion

Using Newton’s second law,

$$
m\ddot{x} = F(x)
$$

we get

$$
m\ddot{x} = -kx - 4\lambda x^3
$$

or equivalently,

$$
\boxed{
m\ddot{x} + kx + 4\lambda x^3 = 0
}
$$

This is a nonlinear oscillator because of the term $x^3$.

---

### 3. First-order system for numerical simulation

To solve numerically, introduce the velocity

$$
v = \dot{x}
$$

Then the second-order equation becomes a system of two first-order equations:

$$
\dot{x} = v
$$

$$
\dot{v} = -\frac{k}{m}x - \frac{4\lambda}{m}x^3
$$

So the numerical model is

$$
\boxed{
\dot{x} = v,\qquad
\dot{v} = -\frac{k}{m}x - \frac{4\lambda}{m}x^3
}
$$

---

### 4. Example of selected parameters

For example, choose

$$
m=1,\qquad k=1,\qquad \lambda=0.1
$$

Then the system becomes

$$
\dot{x}=v
$$

$$
\dot{v}=-x-0.4x^3
$$

with initial conditions, for example,

$$
x(0)=x_0,\qquad v(0)=v_0
$$

These equations can be integrated numerically using Euler’s method, Runge–Kutta, or another standard algorithm.

---

### 5. Effect of the initial energy

The total energy is

$$
E = \frac{1}{2}mv^2 + U(x)
$$

so here

$$
E = \frac{1}{2}mv^2 + \frac{k}{2}x^2 + \lambda x^4
$$

Thus,

$$
\boxed{
E = \frac{1}{2}mv^2 + \frac{k}{2}x^2 + \lambda x^4
}
$$

Since the potential grows for large $|x|$, the particle remains trapped in a bounded region.

The effect of the initial energy is the following:

- for small energy, the motion is close to harmonic,
- for larger energy, the quartic term becomes important,
- the oscillation becomes nonlinear,
- the period depends on the amplitude.

So increasing the initial energy changes the shape of the trajectory and makes the motion less similar to a simple harmonic oscillator.

---

### 6. Qualitative behavior

For small displacements, the quadratic term dominates:

$$
U(x)\approx \frac{k}{2}x^2
$$

and the motion behaves approximately like a harmonic oscillator.

For larger displacements, the term

$$
\lambda x^4
$$

becomes significant, so the restoring force is stronger than in the purely harmonic case.

Therefore, this system is a nonlinear oscillator with bounded motion.

---

### 7. Numerical visualization

A numerical simulation should produce:

1. the graph of position versus time:
   $$
   x(t)
   $$

2. the phase portrait:
   $$
   (x(t),v(t))
   $$

For bounded motion, the phase portrait consists of closed curves around the equilibrium point

$$
x=0,\qquad v=0
$$

For low energy, these curves are close to ellipses.  
For higher energy, they become more distorted because of the nonlinear term.

---

## Conclusion

The potential is

$$
U(x)=\frac{k}{2}x^2+\lambda x^4
$$

The force is

$$
\boxed{
F(x)=-kx-4\lambda x^3
}
$$

The equation of motion is

$$
\boxed{
m\ddot{x}+kx+4\lambda x^3=0
}
$$

The equivalent first-order system is

$$
\boxed{
\dot{x}=v,\qquad
\dot{v}=-\frac{k}{m}x-\frac{4\lambda}{m}x^3
}
$$

The total energy is

$$
\boxed{
E=\frac{1}{2}mv^2+\frac{k}{2}x^2+\lambda x^4
}
$$

The motion is bounded and nonlinear, and the phase portrait consists of closed curves whose shape depends on the initial energy.
