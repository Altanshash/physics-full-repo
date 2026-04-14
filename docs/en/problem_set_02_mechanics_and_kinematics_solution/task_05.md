## Problem 5 – Elliptical motion (purely kinematic)

### Given

The path equation is given in parametric form:

$$
x(t)=a\cos(\omega t), \qquad y(t)=b\sin(\omega t)
$$

Find:

1. Calculate the velocity and acceleration
2. Determine whether the magnitude of the velocity is constant
3. Find where the velocity is maximum
4. Draw the trajectory and the graphs of $|\vec{v}(t)|$ and $|\vec{a}(t)|$

---

### Solution

#### 1. Trajectory

We are given

$$
x(t)=a\cos(\omega t), \qquad y(t)=b\sin(\omega t).
$$

To eliminate the parameter $t$, divide by $a$ and $b$:

$$
\frac{x}{a}=\cos(\omega t), \qquad \frac{y}{b}=\sin(\omega t).
$$

Now square both equations and add them:

$$
\left(\frac{x}{a}\right)^2+\left(\frac{y}{b}\right)^2=\cos^2(\omega t)+\sin^2(\omega t)=1.
$$

Therefore, the trajectory is the ellipse

$$
\boxed{\frac{x^2}{a^2}+\frac{y^2}{b^2}=1}.
$$

---

#### 2. Velocity vector

The velocity vector is

$$
\vec{v}(t)=\left(\frac{dx}{dt},\frac{dy}{dt}\right).
$$

Differentiate the coordinates:

$$
\frac{dx}{dt}=-a\omega\sin(\omega t),
$$

$$
\frac{dy}{dt}=b\omega\cos(\omega t).
$$

Hence,

$$
\boxed{\vec{v}(t)=\bigl(-a\omega\sin(\omega t),\,b\omega\cos(\omega t)\bigr)}.
$$

---

#### 3. Acceleration vector

The acceleration vector is

$$
\vec{a}(t)=\left(\frac{d^2x}{dt^2},\frac{d^2y}{dt^2}\right).
$$

Differentiate once more:

$$
\frac{d^2x}{dt^2}=-a\omega^2\cos(\omega t),
$$

$$
\frac{d^2y}{dt^2}=-b\omega^2\sin(\omega t).
$$

Therefore,

$$
\boxed{\vec{a}(t)=\bigl(-a\omega^2\cos(\omega t),\,-b\omega^2\sin(\omega t)\bigr)}.
$$

---

#### 4. Magnitude of the velocity

The speed is

$$
|\vec{v}(t)|=\sqrt{\left(-a\omega\sin(\omega t)\right)^2+\left(b\omega\cos(\omega t)\right)^2}.
$$

So,

$$
|\vec{v}(t)|=\sqrt{a^2\omega^2\sin^2(\omega t)+b^2\omega^2\cos^2(\omega t)}.
$$

Factor out $\omega^2$:

$$
|\vec{v}(t)|=\omega\sqrt{a^2\sin^2(\omega t)+b^2\cos^2(\omega t)}.
$$

Thus,

$$
\boxed{|\vec{v}(t)|=\omega\sqrt{a^2\sin^2(\omega t)+b^2\cos^2(\omega t)}}.
$$

---

#### 5. Magnitude of the acceleration

The magnitude of the acceleration is

$$
|\vec{a}(t)|=\sqrt{\left(-a\omega^2\cos(\omega t)\right)^2+\left(-b\omega^2\sin(\omega t)\right)^2}.
$$

So,

$$
|\vec{a}(t)|=\sqrt{a^2\omega^4\cos^2(\omega t)+b^2\omega^4\sin^2(\omega t)}.
$$

Factor out $\omega^4$:

$$
|\vec{a}(t)|=\omega^2\sqrt{a^2\cos^2(\omega t)+b^2\sin^2(\omega t)}.
$$

Therefore,

$$
\boxed{|\vec{a}(t)|=\omega^2\sqrt{a^2\cos^2(\omega t)+b^2\sin^2(\omega t)}}.
$$

---

#### 6. Is the magnitude of the velocity constant?

We have

$$
|\vec{v}(t)|=\omega\sqrt{a^2\sin^2(\omega t)+b^2\cos^2(\omega t)}.
$$

This expression depends on time $t$ in general.

Therefore, the magnitude of the velocity is **not constant** unless $a=b$.

If $a=b=R$, then the ellipse becomes a circle and

$$
|\vec{v}(t)|=\omega R,
$$

which is constant.

So, in the general elliptical case,

$$
\boxed{|\vec{v}(t)| \text{ is not constant}.}
$$

---

#### 7. Where is the velocity maximum?

To maximize the speed,

$$
|\vec{v}(t)|=\omega\sqrt{a^2\sin^2(\omega t)+b^2\cos^2(\omega t)},
$$

we need to maximize

$$
a^2\sin^2(\omega t)+b^2\cos^2(\omega t).
$$

The maximum depends on which of $a$ or $b$ is larger.

##### Case 1: $a>b$

Then the maximum occurs when

$$
\sin^2(\omega t)=1, \qquad \cos^2(\omega t)=0.
$$

So,

$$
\omega t=\frac{\pi}{2}+k\pi, \qquad k\in\mathbb{Z}.
$$

At these moments,

$$
x=0,\qquad y=\pm b.
$$

The maximum speed is

$$
|\vec{v}|_{\max}=a\omega.
$$

##### Case 2: $b>a$

Then the maximum occurs when

$$
\cos^2(\omega t)=1, \qquad \sin^2(\omega t)=0.
$$

So,

$$
\omega t=k\pi, \qquad k\in\mathbb{Z}.
$$

At these moments,

$$
x=\pm a,\qquad y=0.
$$

The maximum speed is

$$
|\vec{v}|_{\max}=b\omega.
$$

##### General result

Therefore,

$$
\boxed{|\vec{v}|_{\max}=\omega\max(a,b)}.
$$

So the speed is maximum at the endpoints of the **minor axis**:

- if $a>b$, at $(0,\pm b)$
- if $b>a$, at $(\pm a,0)$

---

#### 8. Graphs of $|\vec{v}(t)|$ and $|\vec{a}(t)|$

The trajectory is the ellipse

$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1.
$$

The graph of the speed is described by

$$
|\vec{v}(t)|=\omega\sqrt{a^2\sin^2(\omega t)+b^2\cos^2(\omega t)},
$$

and the graph of the acceleration magnitude is

$$
|\vec{a}(t)|=\omega^2\sqrt{a^2\cos^2(\omega t)+b^2\sin^2(\omega t)}.
$$

Both are periodic functions of time.

---

### Final Conclusion

For the parametric equations

$$
x(t)=a\cos(\omega t), \qquad y(t)=b\sin(\omega t),
$$

the body moves along the ellipse

$$
\boxed{\frac{x^2}{a^2}+\frac{y^2}{b^2}=1}.
$$

The velocity and acceleration vectors are

$$
\boxed{\vec{v}(t)=\bigl(-a\omega\sin(\omega t),\,b\omega\cos(\omega t)\bigr)}
$$

$$
\boxed{\vec{a}(t)=\bigl(-a\omega^2\cos(\omega t),\,-b\omega^2\sin(\omega t)\bigr)}
$$

Their magnitudes are

$$
\boxed{|\vec{v}(t)|=\omega\sqrt{a^2\sin^2(\omega t)+b^2\cos^2(\omega t)}}
$$

$$
\boxed{|\vec{a}(t)|=\omega^2\sqrt{a^2\cos^2(\omega t)+b^2\sin^2(\omega t)}}
$$

Thus, in general, the speed is **not constant**, and its maximum value is

$$
\boxed{|\vec{v}|_{\max}=\omega\max(a,b)}.
$$

The maximum speed is reached at the endpoints of the **minor axis** of the ellipse.
