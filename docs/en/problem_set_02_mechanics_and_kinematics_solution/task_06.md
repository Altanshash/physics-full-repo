## Problem 6 – Cycloid: trajectory of a point on a rolling circle

### Given

A circle of radius $R$ rolls without slipping along the $x$-axis.  
A point on the rim of the circle traces a cycloid:

$$
x(t)=R\bigl(\omega t-\sin(\omega t)\bigr), \qquad
y(t)=R\bigl(1-\cos(\omega t)\bigr)
$$

Find:

1. Determine the velocity vector $\vec{v}(t)$ and the acceleration vector $\vec{a}(t)$
2. Calculate $|\vec{v}(t)|$ and indicate the moments when the point temporarily stops relative to the ground
3. Determine the maximum values of $|\vec{v}|$ and $|\vec{a}|$
4. Compare the cycloid with circular motion in a reference frame attached to the circle

---

### Solution

#### 1. Position vector

The position vector is

$$
\vec{r}(t)=\bigl(x(t),y(t)\bigr)
=\left(R(\omega t-\sin(\omega t)),\;R(1-\cos(\omega t))\right).
$$

---

#### 2. Velocity vector

The velocity vector is

$$
\vec{v}(t)=\left(\frac{dx}{dt},\frac{dy}{dt}\right).
$$

Differentiate the coordinates:

$$
\frac{dx}{dt}=R\omega\bigl(1-\cos(\omega t)\bigr),
$$

$$
\frac{dy}{dt}=R\omega\sin(\omega t).
$$

Hence,

$$
\boxed{
\vec{v}(t)=\left(R\omega(1-\cos(\omega t)),\;R\omega\sin(\omega t)\right)
}.
$$

---

#### 3. Acceleration vector

The acceleration vector is

$$
\vec{a}(t)=\left(\frac{d^2x}{dt^2},\frac{d^2y}{dt^2}\right).
$$

Differentiate once more:

$$
\frac{d^2x}{dt^2}=R\omega^2\sin(\omega t),
$$

$$
\frac{d^2y}{dt^2}=R\omega^2\cos(\omega t).
$$

Therefore,

$$
\boxed{
\vec{a}(t)=\left(R\omega^2\sin(\omega t),\;R\omega^2\cos(\omega t)\right)
}.
$$

---

#### 4. Magnitude of the velocity

The speed is

$$
|\vec{v}(t)|=
\sqrt{\left(R\omega(1-\cos(\omega t))\right)^2+\left(R\omega\sin(\omega t)\right)^2}.
$$

Factor out $R\omega$:

$$
|\vec{v}(t)|=
R\omega\sqrt{(1-\cos(\omega t))^2+\sin^2(\omega t)}.
$$

Expand the expression inside the square root:

$$
(1-\cos(\omega t))^2+\sin^2(\omega t)
=1-2\cos(\omega t)+\cos^2(\omega t)+\sin^2(\omega t).
$$

Using

$$
\cos^2(\omega t)+\sin^2(\omega t)=1,
$$

we obtain

$$
(1-\cos(\omega t))^2+\sin^2(\omega t)=2-2\cos(\omega t).
$$

Thus,

$$
|\vec{v}(t)|=R\omega\sqrt{2-2\cos(\omega t)}.
$$

Using the identity

$$
2-2\cos(\omega t)=4\sin^2\left(\frac{\omega t}{2}\right),
$$

we get

$$
\boxed{
|\vec{v}(t)|=2R\omega\left|\sin\left(\frac{\omega t}{2}\right)\right|
}.
$$

---

#### 5. Moments when the point temporarily stops

The point stops relative to the ground when

$$
|\vec{v}(t)|=0.
$$

From

$$
|\vec{v}(t)|=2R\omega\left|\sin\left(\frac{\omega t}{2}\right)\right|,
$$

this occurs when

$$
\sin\left(\frac{\omega t}{2}\right)=0.
$$

Hence,

$$
\frac{\omega t}{2}=k\pi,
\qquad k\in\mathbb{Z},
$$

so

$$
\boxed{
t=\frac{2\pi k}{\omega}, \qquad k\in\mathbb{Z}
}.
$$

These moments correspond to the cusp points of the cycloid.

---

#### 6. Maximum value of the speed

Since

$$
|\vec{v}(t)|=2R\omega\left|\sin\left(\frac{\omega t}{2}\right)\right|,
$$

the maximum speed occurs when

$$
\left|\sin\left(\frac{\omega t}{2}\right)\right|=1.
$$

Therefore,

$$
\boxed{
|\vec{v}|_{\max}=2R\omega
}.
$$

This happens when

$$
\frac{\omega t}{2}=\frac{\pi}{2}+k\pi,
\qquad k\in\mathbb{Z},
$$

that is,

$$
\boxed{
t=\frac{(2k+1)\pi}{\omega}, \qquad k\in\mathbb{Z}
}.
$$

---

#### 7. Magnitude of the acceleration

The magnitude of the acceleration is

$$
|\vec{a}(t)|=
\sqrt{\left(R\omega^2\sin(\omega t)\right)^2+\left(R\omega^2\cos(\omega t)\right)^2}.
$$

Factor out $R\omega^2$:

$$
|\vec{a}(t)|=
R\omega^2\sqrt{\sin^2(\omega t)+\cos^2(\omega t)}.
$$

Since

$$
\sin^2(\omega t)+\cos^2(\omega t)=1,
$$

we obtain

$$
\boxed{
|\vec{a}(t)|=R\omega^2
}.
$$

So the acceleration magnitude is constant, and therefore

$$
\boxed{
|\vec{a}|_{\max}=R\omega^2
}.
$$

---

#### 8. Comparison with circular motion in the frame attached to the circle

In the ground reference frame, the point moves along a cycloid.

Now consider a reference frame attached to the center of the rolling circle.  
The center has coordinates

$$
C(t)=\bigl(R\omega t,\;R\bigr).
$$

Relative to this center, the point has coordinates

$$
x'(t)=x(t)-R\omega t=-R\sin(\omega t),
$$

$$
y'(t)=y(t)-R=-R\cos(\omega t).
$$

Therefore,

$$
x'^2(t)+y'^2(t)=R^2\sin^2(\omega t)+R^2\cos^2(\omega t)=R^2.
$$

So in the moving frame,

$$
\boxed{x'^2+y'^2=R^2},
$$

which is the equation of a circle.

Thus:

- in the **ground frame**, the trajectory is a **cycloid**
- in the **frame attached to the circle**, the motion is **uniform circular motion**

---

### Final Conclusion

For the cycloid defined by

$$
x(t)=R(\omega t-\sin(\omega t)), \qquad
y(t)=R(1-\cos(\omega t)),
$$

the position, velocity, and acceleration vectors are

$$
\boxed{
\vec{r}(t)=\left(R(\omega t-\sin(\omega t)),\;R(1-\cos(\omega t))\right)
}
$$

$$
\boxed{
\vec{v}(t)=\left(R\omega(1-\cos(\omega t)),\;R\omega\sin(\omega t)\right)
}
$$

$$
\boxed{
\vec{a}(t)=\left(R\omega^2\sin(\omega t),\;R\omega^2\cos(\omega t)\right)
}
$$

Their magnitudes are

$$
\boxed{
|\vec{v}(t)|=2R\omega\left|\sin\left(\frac{\omega t}{2}\right)\right|
}
$$

$$
\boxed{
|\vec{a}(t)|=R\omega^2
}
$$

The point temporarily stops at

$$
\boxed{
t=\frac{2\pi k}{\omega}, \qquad k\in\mathbb{Z}
}
$$

The maximum values are

$$
\boxed{
|\vec{v}|_{\max}=2R\omega
}
\qquad
\boxed{
|\vec{a}|_{\max}=R\omega^2
}
$$

Therefore, the cycloid is obtained as the result of the combination of translational motion of the circle’s center and circular motion of the point relative to that center.
