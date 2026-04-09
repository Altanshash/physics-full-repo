## Problem 10 – Numerical model of a dynamical system

### Problem statement

Given the potential

$$
U(x)=\frac{k}{2}x^2+\lambda x^4
$$

Find:

- the force,
- the equation of motion,
- the numerical form of the system,
- the effect of initial energy,
- the plots of $x(t)$ and the phase portrait.

---

## Solution

### 1. Force

The force is

$$
F(x)=-\frac{dU}{dx}
$$

Differentiate the potential:

$$
\frac{dU}{dx}=\frac{d}{dx}\left(\frac{k}{2}x^2+\lambda x^4\right)
$$

$$
\frac{dU}{dx}=kx+4\lambda x^3
$$

Therefore,

$$
\boxed{F(x)=-kx-4\lambda x^3}
$$

---

### 2. Equation of motion

Using Newton’s second law,

$$
m\ddot{x}=F(x)
$$

Substitute the force:

$$
m\ddot{x}=-kx-4\lambda x^3
$$

Move everything to one side:

$$
\boxed{m\ddot{x}+kx+4\lambda x^3=0}
$$

---

### 3. First-order system for numerical solution

Let

$$
v=\dot{x}
$$

Then

$$
\dot{x}=v
$$

Also,

$$
\dot{v}=\ddot{x}
$$

From the equation of motion:

$$
m\dot{v}=-kx-4\lambda x^3
$$

Divide by $m$:

$$
\dot{v}=-\frac{k}{m}x-\frac{4\lambda}{m}x^3
$$

So the numerical system is

$$
\boxed{\dot{x}=v}
$$

$$
\boxed{\dot{v}=-\frac{k}{m}x-\frac{4\lambda}{m}x^3}
$$

---

### 4. Total energy

The total energy is

$$
E=\frac{1}{2}mv^2+U(x)
$$

Substitute $U(x)$:

$$
E=\frac{1}{2}mv^2+\frac{k}{2}x^2+\lambda x^4
$$

Therefore,

$$
\boxed{E=\frac{1}{2}mv^2+\frac{k}{2}x^2+\lambda x^4}
$$

---

### 5. Effect of initial energy

If the initial energy is small, then $x$ is small, so the term $\lambda x^4$ is much smaller than $\frac{k}{2}x^2$.

Then the motion is approximately harmonic.

If the initial energy is larger, then $x$ becomes larger, and the term $\lambda x^4$ becomes important.

So:

- small energy → almost harmonic motion,
- large energy → nonlinear motion,
- larger energy → larger amplitude and more distorted phase curves.

---

### 6. Numerical example

Choose, for example,

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

with initial conditions

$$
x(0)=x_0,\qquad v(0)=v_0
$$

---

### 7. What to plot

For the numerical solution, plot:

1. position versus time:

$$
x(t)
$$

2. phase portrait:

$$
(x(t),v(t))
$$

For bounded motion, the phase portrait consists of closed curves around

$$
x=0,\qquad v=0
$$

---

## Conclusion

The force is

$$
\boxed{F(x)=-kx-4\lambda x^3}
$$

The equation of motion is

$$
\boxed{m\ddot{x}+kx+4\lambda x^3=0}
$$

The first-order system is

$$
\boxed{\dot{x}=v,\qquad \dot{v}=-\frac{k}{m}x-\frac{4\lambda}{m}x^3}
$$

The total energy is

$$
\boxed{E=\frac{1}{2}mv^2+\frac{k}{2}x^2+\lambda x^4}
$$

The motion is bounded and nonlinear.
