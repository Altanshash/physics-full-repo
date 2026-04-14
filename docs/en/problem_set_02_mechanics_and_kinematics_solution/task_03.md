## Problem 3 – Elimination of time and interpretation of acceleration

### Given

The motion is given in parametric form:

$$
x(t)=2t^2,\qquad y(t)=3t^3
$$

Find:

1. Eliminate the parameter $t$
2. Draw the trajectory
3. Calculate $\vec{v}(t)$, $|\vec{v}(t)|$, $\vec{a}(t)$ and $|\vec{a}(t)|$
4. Determine whether the acceleration is constant

---

### Solution

#### 1. Eliminate the parameter $t$

From

$$
x=2t^2
$$

we get

$$
t^2=\frac{x}{2}.
$$

Also,

$$
y=3t^3.
$$

Now square both sides of the second equation:

$$
y^2=9t^6.
$$

Since

$$
t^6=(t^2)^3,
$$

we substitute $t^2=\dfrac{x}{2}$:

$$
t^6=\left(\frac{x}{2}\right)^3=\frac{x^3}{8}.
$$

Therefore,

$$
y^2=9\cdot\frac{x^3}{8}=\frac{9}{8}x^3.
$$

So, after eliminating the parameter $t$, the trajectory equation is

$$
\boxed{y^2=\frac{9}{8}x^3}, \qquad x\ge0.
$$

---

#### 2. Trajectory

The trajectory is described by the equation

$$
y^2=\frac{9}{8}x^3, \qquad x\ge0.
$$

This is a **semicubical parabola** opening to the right.

- At $t=0$, the particle is at the origin:
  $$
  (x,y)=(0,0)
  $$
- For $t>0$, we have $y>0$, so the particle moves along the **upper branch**
- For $t<0$, we have $y<0$, so the particle moves along the **lower branch**

---

#### 3. Velocity and acceleration

##### Velocity vector

The velocity vector is

$$
\vec{v}(t)=\left(\frac{dx}{dt},\frac{dy}{dt}\right).
$$

Differentiate the coordinates:

$$
\frac{dx}{dt}=4t,\qquad \frac{dy}{dt}=9t^2.
$$

Hence,

$$
\boxed{\vec{v}(t)=(4t,\,9t^2)}.
$$

---

##### Magnitude of velocity

The speed is

$$
|\vec{v}(t)|=\sqrt{(4t)^2+(9t^2)^2}.
$$

So,

$$
|\vec{v}(t)|=\sqrt{16t^2+81t^4}.
$$

Therefore,

$$
\boxed{|\vec{v}(t)|=\sqrt{16t^2+81t^4}}.
$$

---

##### Acceleration vector

The acceleration vector is

$$
\vec{a}(t)=\left(\frac{d^2x}{dt^2},\frac{d^2y}{dt^2}\right).
$$

Differentiate once more:

$$
\frac{d^2x}{dt^2}=4,\qquad \frac{d^2y}{dt^2}=18t.
$$

Hence,

$$
\boxed{\vec{a}(t)=(4,\,18t)}.
$$

---

##### Magnitude of acceleration

The magnitude of acceleration is

$$
|\vec{a}(t)|=\sqrt{4^2+(18t)^2}.
$$

Thus,

$$
|\vec{a}(t)|=\sqrt{16+324t^2}.
$$

Therefore,

$$
\boxed{|\vec{a}(t)|=\sqrt{16+324t^2}}.
$$

---

#### 4. Is the acceleration constant?

The acceleration vector is

$$
\vec{a}(t)=(4,18t).
$$

Its first component is constant, but its second component depends on time $t$.

Therefore, the acceleration vector changes with time, so it is **not constant**.

---

### Final Conclusion

For the parametric equations

$$
x(t)=2t^2,\qquad y(t)=3t^3,
$$

the parameter elimination gives the trajectory

$$
\boxed{y^2=\frac{9}{8}x^3}, \qquad x\ge0.
$$

The velocity and acceleration are

$$
\boxed{\vec{v}(t)=(4t,\,9t^2)}
$$

$$
\boxed{|\vec{v}(t)|=\sqrt{16t^2+81t^4}}
$$

$$
\boxed{\vec{a}(t)=(4,\,18t)}
$$

$$
\boxed{|\vec{a}(t)|=\sqrt{16+324t^2}}
$$

Thus, the particle moves along a semicubical parabola, and the acceleration is

$$
\boxed{\text{not constant}}.
$$
