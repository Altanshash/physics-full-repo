## Problem 2 – Projectile motion

### Problem statement

A body moves in the Earth's gravitational field without air resistance.  
It is thrown with initial velocity $v_0$ at an angle $\alpha$ to the horizontal.

Determine:

- the equations of motion in the horizontal and vertical directions,
- the time of flight,
- the maximum height,
- the range,
- the angle for which the range is maximum.

---

## Solution

### 1. Initial velocity components

Resolve the initial velocity into horizontal and vertical components:

$$
v_{0x}=v_0\cos\alpha
$$

$$
v_{0y}=v_0\sin\alpha
$$

The horizontal acceleration is zero:

$$
a_x=0
$$

The vertical acceleration is

$$
a_y=-g
$$

---

### 2. Equations of motion

#### Horizontal motion

Since $a_x=0$, the horizontal velocity is constant:

$$
v_x(t)=v_0\cos\alpha
$$

Therefore, the horizontal position is

$$
x(t)=v_0\cos\alpha \, t
$$

#### Vertical motion

The vertical velocity is

$$
v_y(t)=v_0\sin\alpha - gt
$$

The vertical position is

$$
y(t)=v_0\sin\alpha \, t - \frac{1}{2}gt^2
$$

So the equations of motion are

$$
\boxed{x(t)=v_0\cos\alpha \, t}
$$

$$
\boxed{y(t)=v_0\sin\alpha \, t - \frac{1}{2}gt^2}
$$

---

### 3. Time of flight

The body lands when it returns to the ground, so

$$
y(t)=0
$$

Substitute the vertical position:

$$
v_0\sin\alpha \, t - \frac{1}{2}gt^2=0
$$

Factor out $t$:

$$
t\left(v_0\sin\alpha - \frac{1}{2}gt\right)=0
$$

One solution is $t=0$, which is the launch time.  
The second solution gives the time of flight:

$$
v_0\sin\alpha - \frac{1}{2}gt=0
$$

$$
\frac{1}{2}gt=v_0\sin\alpha
$$

$$
t=\frac{2v_0\sin\alpha}{g}
$$

Therefore,

$$
\boxed{T=\frac{2v_0\sin\alpha}{g}}
$$

---

### 4. Maximum height

At the highest point, the vertical velocity becomes zero:

$$
v_y(t)=0
$$

So,

$$
v_0\sin\alpha - gt=0
$$

Hence,

$$
t_h=\frac{v_0\sin\alpha}{g}
$$

Now substitute this into the vertical position formula:

$$
H_{\max}=v_0\sin\alpha \cdot \frac{v_0\sin\alpha}{g}
-\frac{1}{2}g\left(\frac{v_0\sin\alpha}{g}\right)^2
$$

Simplify the first term:

$$
\frac{v_0^2\sin^2\alpha}{g}
$$

Simplify the second term:

$$
\frac{1}{2}\frac{v_0^2\sin^2\alpha}{g}
$$

So,

$$
H_{\max}
=
\frac{v_0^2\sin^2\alpha}{g}
-
\frac{1}{2}\frac{v_0^2\sin^2\alpha}{g}
$$

$$
H_{\max}
=
\frac{v_0^2\sin^2\alpha}{2g}
$$

Therefore,

$$
\boxed{H_{\max}=\frac{v_0^2\sin^2\alpha}{2g}}
$$

---

### 5. Range

The range is the horizontal distance at time $T$:

$$
R=x(T)
$$

Using

$$
x(t)=v_0\cos\alpha \, t
$$

and

$$
T=\frac{2v_0\sin\alpha}{g}
$$

we get

$$
R=v_0\cos\alpha \cdot \frac{2v_0\sin\alpha}{g}
$$

So,

$$
R=\frac{2v_0^2\sin\alpha\cos\alpha}{g}
$$

Use the identity

$$
2\sin\alpha\cos\alpha=\sin 2\alpha
$$

Then

$$
\boxed{R=\frac{v_0^2\sin 2\alpha}{g}}
$$

---

### 6. Angle for maximum range

The range is

$$
R=\frac{v_0^2\sin 2\alpha}{g}
$$

For fixed $v_0$ and $g$, the range is maximum when $\sin 2\alpha$ is maximum.

The maximum value of sine is 1, so

$$
\sin 2\alpha = 1
$$

This happens when

$$
2\alpha=90^\circ
$$

Hence,

$$
\alpha=45^\circ
$$

Therefore,

$$
\boxed{\alpha=45^\circ}
$$

---

## Conclusion

The projectile motion is described by

$$
\boxed{x(t)=v_0\cos\alpha \, t}
$$

$$
\boxed{y(t)=v_0\sin\alpha \, t - \frac{1}{2}gt^2}
$$

The time of flight is

$$
\boxed{T=\frac{2v_0\sin\alpha}{g}}
$$

The maximum height is

$$
\boxed{H_{\max}=\frac{v_0^2\sin^2\alpha}{2g}}
$$

The range is

$$
\boxed{R=\frac{v_0^2\sin 2\alpha}{g}}
$$

The range is maximum for

$$
\boxed{\alpha=45^\circ}
$$
