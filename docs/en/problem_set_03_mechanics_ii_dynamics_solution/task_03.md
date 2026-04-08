## Problem 3 – Work of a variable force

### Given

A one-dimensional force is given by

$$
F(x) = -kx
$$

where $k>0$ is a constant.

We need to:

- write down the equation of motion and solve it,
- calculate the work done during the displacement from $0$ to $x_0$,
- interpret the result as potential energy,
- verify the relation $F = -\dfrac{dU}{dx}$,
- describe the graphs of $F(x)$ and $U(x)$.

---

## 1. Equation of motion

Using Newton’s second law,

$$
m\ddot{x} = F(x)
$$

and substituting $F(x)=-kx$, we obtain

$$
m\ddot{x} = -kx
$$

or equivalently

$$
\ddot{x} + \frac{k}{m}x = 0
$$

This is the differential equation of a simple harmonic oscillator.

Let

$$
\omega = \sqrt{\frac{k}{m}}
$$

Then the equation becomes

$$
\ddot{x} + \omega^2 x = 0
$$

The general solution is

$$
x(t) = A\cos(\omega t) + B\sin(\omega t)
$$

where $A$ and $B$ are constants determined by the initial conditions.

Thus, the motion is oscillatory.

---

## 2. Work done from $0$ to $x_0$

The work done by a variable force is

$$
W = \int_0^{x_0} F(x)\,dx
$$

Substitute $F(x)=-kx$:

$$
W = \int_0^{x_0} (-kx)\,dx
$$

Take the constant $-k$ outside the integral:

$$
W = -k\int_0^{x_0} x\,dx
$$

Now integrate:

$$
\int_0^{x_0} x\,dx = \left[\frac{x^2}{2}\right]_0^{x_0} = \frac{x_0^2}{2}
$$

Therefore,

$$
W = -k\cdot \frac{x_0^2}{2}
$$

So the work done by the force is

$$
\boxed{W = -\frac{1}{2}kx_0^2}
$$

This result is negative because the force is directed opposite to the displacement when $x_0>0$.

---

## 3. Interpretation as potential energy

For a conservative force, the work is related to the change in potential energy by

$$
W = -\Delta U
$$

If we choose the reference value

$$
U(0)=0
$$

then the potential energy at position $x$ is

$$
U(x) = \frac{1}{2}kx^2
$$

In particular, at $x=x_0$,

$$
U(x_0)=\frac{1}{2}kx_0^2
$$

Thus,

$$
W(0\to x_0) = -\left(U(x_0)-U(0)\right)
= -\frac{1}{2}kx_0^2
$$

which agrees with the previous result.

Hence, the potential energy associated with the force $F(x)=-kx$ is

$$
\boxed{U(x)=\frac{1}{2}kx^2}
$$

---

## 4. Verification of the relation $F=-\dfrac{dU}{dx}$

We found that

$$
U(x)=\frac{1}{2}kx^2
$$

Differentiate with respect to $x$:

$$
\frac{dU}{dx} = kx
$$

Now take the negative sign:

$$
-\frac{dU}{dx} = -kx
$$

But this is exactly the given force:

$$
F(x)=-kx
$$

Therefore,

$$
\boxed{F = -\frac{dU}{dx}}
$$

is verified.

---

## 5. Graphs of $F(x)$ and $U(x)$

### Graph of $F(x)$

The function

$$
F(x)=-kx
$$

is a straight line passing through the origin with negative slope $-k$.

- if $x>0$, then $F(x)<0$,
- if $x<0$, then $F(x)>0$.

So the force always points toward the equilibrium position $x=0$.

### Graph of $U(x)$

The function

$$
U(x)=\frac{1}{2}kx^2
$$

is an upward-opening parabola with minimum at $x=0$.

- $U(x)\ge 0$ for all $x$,
- the minimum potential energy occurs at the equilibrium point.

Thus, the system behaves like a spring, and $x=0$ is a stable equilibrium position.

---

## Final answers

$$
\boxed{m\ddot{x}=-kx}
$$

$$
\boxed{\ddot{x}+\frac{k}{m}x=0}
$$

$$
\boxed{x(t)=A\cos\left(\sqrt{\frac{k}{m}}\,t\right)+B\sin\left(\sqrt{\frac{k}{m}}\,t\right)}
$$

$$
\boxed{W(0\to x_0)=-\frac{1}{2}kx_0^2}
$$

$$
\boxed{U(x)=\frac{1}{2}kx^2}
$$

$$
\boxed{F=-\frac{dU}{dx}}
$$
