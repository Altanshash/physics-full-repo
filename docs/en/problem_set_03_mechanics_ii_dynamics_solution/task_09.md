## Problem 9 – Potential and conservative field

### Problem statement

The potential energy is given by

$$
U(x,y) = \frac{k}{2}(x^2 + y^2)
$$

Determine:

- the force as the gradient of the potential,
- the equations of motion,
- the type of motion,
- the total energy,
- the geometrical interpretation of the trajectory.

---

## Solution

### 1. Force from the potential

The force is the negative gradient of the potential:

$$
\vec{F} = -\nabla U
$$

Compute the partial derivatives:

$$
\frac{\partial U}{\partial x} = kx,
\qquad
\frac{\partial U}{\partial y} = ky
$$

Therefore,

$$
\vec{F}(x,y) = (-kx,\,-ky)
$$

So,

$$
\boxed{\vec{F}(x,y)=(-kx,\,-ky)}
$$

---

### 2. Equations of motion

Using Newton’s second law,

$$
m\ddot{x} = F_x = -kx
$$

$$
m\ddot{y} = F_y = -ky
$$

Hence,

$$
\ddot{x} + \frac{k}{m}x = 0
$$

$$
\ddot{y} + \frac{k}{m}y = 0
$$

Introduce

$$
\omega^2 = \frac{k}{m}
$$

Then the equations become

$$
\ddot{x} + \omega^2 x = 0
$$

$$
\ddot{y} + \omega^2 y = 0
$$

---

### 3. General solution

Each coordinate satisfies the harmonic oscillator equation.

So,

$$
x(t) = A\cos(\omega t) + B\sin(\omega t)
$$

$$
y(t) = C\cos(\omega t) + D\sin(\omega t)
$$

Thus, the motion in two dimensions is a combination of two harmonic oscillations with the same frequency.

---

### 4. Type of motion

Because both coordinates oscillate with the same angular frequency,

$$
\omega = \sqrt{\frac{k}{m}},
$$

the motion is a **two-dimensional harmonic motion** in a central conservative field.

Depending on the constants $A,B,C,D$, the trajectory can be:

- a line,
- an ellipse,
- a circle.

So the motion is bounded and periodic.

---

### 5. Total energy

The kinetic energy is

$$
T = \frac{m}{2}(\dot{x}^2 + \dot{y}^2)
$$

The potential energy is

$$
U = \frac{k}{2}(x^2 + y^2)
$$

Therefore, the total energy is

$$
E = T + U
$$

that is,

$$
E = \frac{m}{2}(\dot{x}^2 + \dot{y}^2) + \frac{k}{2}(x^2 + y^2)
$$

So,

$$
\boxed{
E = \frac{m}{2}(\dot{x}^2 + \dot{y}^2) + \frac{k}{2}(x^2 + y^2)
}
$$

Since the force is conservative, this energy is constant.

---

### 6. Geometrical interpretation

The potential

$$
U(x,y)=\frac{k}{2}(x^2+y^2)
$$

depends only on the distance from the origin:

$$
r^2 = x^2 + y^2
$$

So the force always points toward the origin:

$$
\vec{F}=(-kx,-ky)
$$

This means the origin is a stable equilibrium point.

The particle moves in a bounded orbit around the origin.  
In general, the trajectory is an ellipse.  
If the amplitudes are equal and the phase shift is suitable, the trajectory becomes a circle.

Thus, geometrically, the system is an isotropic two-dimensional harmonic oscillator.

---

## Conclusion

The force is

$$
\boxed{\vec{F}(x,y)=(-kx,-ky)}
$$

The equations of motion are

$$
\boxed{\ddot{x}+\frac{k}{m}x=0}
$$

$$
\boxed{\ddot{y}+\frac{k}{m}y=0}
$$

The motion is a two-dimensional harmonic motion with frequency

$$
\boxed{\omega=\sqrt{\frac{k}{m}}}
$$

The total energy is

$$
\boxed{
E=\frac{m}{2}(\dot{x}^2+\dot{y}^2)+\frac{k}{2}(x^2+y^2)
}
$$

The trajectory is bounded and is generally an ellipse centered at the origin.
