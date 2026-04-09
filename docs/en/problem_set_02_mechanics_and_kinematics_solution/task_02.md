## Problem 2 – Projectile motion

### Problem statement

A body moves in the Earth's gravitational field without air resistance.  
It is launched with initial speed $v_0$ at an angle $\alpha$ to the horizontal.

Find:

- the equations of motion in the horizontal and vertical directions,
- the time of flight,
- the maximum height,
- the range,
- the angle for which the range is maximum.

---

## Solution

### 1. Initial velocity components

The initial velocity is decomposed into two components:

$$
v_{0x} = v_0 \cos\alpha
$$

$$
v_{0y} = v_0 \sin\alpha
$$

The accelerations are

$$
a_x = 0
$$

$$
a_y = -g
$$

---

### 2. Equations of motion

#### Horizontal motion

Since the horizontal acceleration is zero, the horizontal velocity is constant:

$$
v_x(t) = v_0 \cos\alpha
$$

So the horizontal position is

$$
x(t) = v_0 \cos\alpha \, t
$$

#### Vertical motion

The vertical velocity is

$$
v_y(t) = v_0 \sin\alpha - gt
$$

The vertical position is

$$
y(t) = v_0 \sin\alpha \, t - \frac{1}{2}gt^2
$$

Therefore,

$$
\boxed{x(t)=v_0\cos\alpha \, t}
$$

$$
\boxed{y(t)=v_0\sin\alpha \, t-\frac{1}{2}gt^2}
$$

---

### 3. Time of flight

The projectile returns to the ground when

$$
y(t)=0
$$

Substitute the expression for $y(t)$:

$$
v_0\sin\alpha \, t - \frac{1}{2}gt^2 = 0
$$

Factor out $t$:

$$
t\left(v_0\sin\alpha - \frac{1}{2}gt\right)=0
$$

The nonzero solution gives the total flight time:

$$
v_0\sin\alpha - \frac{1}{2}gt = 0
$$

$$
\frac{1}{2}gt = v_0\sin\alpha
$$

$$
T = \frac{2v_0\sin\alpha}{g}
$$

So,

$$
\boxed{T=\frac{2v_0\sin\alpha}{g}}
$$

---

### 4. Maximum height

At the highest point, the vertical velocity is zero:

$$
v_y(t)=0
$$

Thus,

$$
v_0\sin\alpha - gt = 0
$$

So the time to reach the highest point is

$$
t_h = \frac{v_0\sin\alpha}{g}
$$

Now substitute this into $y(t)$:

$$
H_{\max} = v_0\sin\alpha \cdot \frac{v_0\sin\alpha}{g} - \frac{1}{2}g\left(\frac{v_0\sin\alpha}{g}\right)^2
$$

Simplify the first term:

$$
\frac{v_0^2\sin^2\alpha}{g}
$$

Simplify the second term:

$$
\frac{1}{2}\frac{v_0^2\sin^2\alpha}{g}
$$

Therefore,

$$
H_{\max} = \frac{v_0^2\sin^2\alpha}{g} - \frac{1}{2}\frac{v_0^2\sin^2\alpha}{g}
$$

$$
H_{\max} = \frac{v_0^2\sin^2\alpha}{2g}
$$

Hence,

$$
\boxed{H_{\max}=\frac{v_0^2\sin^2\alpha}{2g}}
$$

---

### 5. Range

The range is the horizontal distance traveled during the full flight time:

$$
R = x(T)
$$

Using

$$
x(t)=v_0\cos\alpha \, t
$$

we get

$$
R = v_0\cos\alpha \cdot \frac{2v_0\sin\alpha}{g}
$$

So,

$$
R = \frac{2v_0^2\sin\alpha\cos\alpha}{g}
$$

Using the identity

$$
\sin 2\alpha = 2\sin\alpha\cos\alpha
$$

we obtain

$$
\boxed{R=\frac{v_0^2\sin 2\alpha}{g}}
$$

---

### 6. Angle for maximum range

The range is

$$
R=\frac{v_0^2\sin 2\alpha}{g}
$$

For fixed $v_0$ and $g$, the range is maximum when $\sin 2\alpha = 1$.

This happens when

$$
2\alpha = 90^\circ
$$

Therefore,

$$
\boxed{\alpha = 45^\circ}
$$

---

## Conclusion

The equations of motion are

$$
\boxed{x(t)=v_0\cos\alpha \, t}
$$

$$
\boxed{y(t)=v_0\sin\alpha \, t-\frac{1}{2}gt^2}
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

The maximum range is obtained for

$$
\boxed{\alpha=45^\circ}
$$
