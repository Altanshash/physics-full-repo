## Problem 4 – Circular motion

### Given

A body moves in a circle of radius $R$ with angular velocity $\omega$.

The position vector can be written as

$$
\vec{r}(t)=\bigl(R\cos(\omega t),\,R\sin(\omega t)\bigr).
$$

Find:

1. Determine $\vec{r}(t)$, $\vec{v}(t)$, $\vec{a}(t)$
2. Determine $|\vec{r}(t)|$, $|\vec{v}(t)|$, $|\vec{a}(t)|$
3. Show that the acceleration is centripetal
4. Visualize the vectors $\vec{r}$, $\vec{v}$, $\vec{a}$

---

### Solution

#### 1. Position vector

For circular motion of radius $R$ with angular velocity $\omega$, the position vector is

$$
\boxed{\vec{r}(t)=\bigl(R\cos(\omega t),\,R\sin(\omega t)\bigr)}.
$$

This describes a circle centered at the origin.

---

#### 2. Velocity vector

The velocity vector is the derivative of the position vector:

$$
\vec{v}(t)=\frac{d\vec{r}}{dt}.
$$

Differentiate each component:

$$
\frac{d}{dt}\bigl(R\cos(\omega t)\bigr)=-R\omega\sin(\omega t),
$$

$$
\frac{d}{dt}\bigl(R\sin(\omega t)\bigr)=R\omega\cos(\omega t).
$$

Therefore,

$$
\boxed{\vec{v}(t)=\bigl(-R\omega\sin(\omega t),\,R\omega\cos(\omega t)\bigr)}.
$$

---

#### 3. Acceleration vector

The acceleration vector is the derivative of the velocity vector:

$$
\vec{a}(t)=\frac{d\vec{v}}{dt}.
$$

Differentiate again:

$$
\frac{d}{dt}\bigl(-R\omega\sin(\omega t)\bigr)=-R\omega^2\cos(\omega t),
$$

$$
\frac{d}{dt}\bigl(R\omega\cos(\omega t)\bigr)=-R\omega^2\sin(\omega t).
$$

Hence,

$$
\boxed{\vec{a}(t)=\bigl(-R\omega^2\cos(\omega t),\,-R\omega^2\sin(\omega t)\bigr)}.
$$

---

#### 4. Magnitudes of the vectors

##### Magnitude of the position vector

$$
|\vec{r}(t)|=\sqrt{(R\cos(\omega t))^2+(R\sin(\omega t))^2}.
$$

Using $\cos^2(\omega t)+\sin^2(\omega t)=1$, we get

$$
|\vec{r}(t)|=\sqrt{R^2}=R.
$$

So,

$$
\boxed{|\vec{r}(t)|=R}.
$$

---

##### Magnitude of the velocity vector

$$
|\vec{v}(t)|=\sqrt{(-R\omega\sin(\omega t))^2+(R\omega\cos(\omega t))^2}.
$$

$$
|\vec{v}(t)|=\sqrt{R^2\omega^2\bigl(\sin^2(\omega t)+\cos^2(\omega t)\bigr)}.
$$

Therefore,

$$
|\vec{v}(t)|=\sqrt{R^2\omega^2}=R\omega.
$$

So,

$$
\boxed{|\vec{v}(t)|=R\omega}.
$$

---

##### Magnitude of the acceleration vector

$$
|\vec{a}(t)|=\sqrt{(-R\omega^2\cos(\omega t))^2+(-R\omega^2\sin(\omega t))^2}.
$$

$$
|\vec{a}(t)|=\sqrt{R^2\omega^4\bigl(\cos^2(\omega t)+\sin^2(\omega t)\bigr)}.
$$

Thus,

$$
|\vec{a}(t)|=\sqrt{R^2\omega^4}=R\omega^2.
$$

Hence,

$$
\boxed{|\vec{a}(t)|=R\omega^2}.
$$

---

#### 5. Show that the acceleration is centripetal

From the expression for $\vec{a}(t)$,

$$
\vec{a}(t)=\bigl(-R\omega^2\cos(\omega t),\,-R\omega^2\sin(\omega t)\bigr).
$$

Factor out $-\omega^2$:

$$
\vec{a}(t)=-\omega^2\bigl(R\cos(\omega t),\,R\sin(\omega t)\bigr).
$$

But

$$
\vec{r}(t)=\bigl(R\cos(\omega t),\,R\sin(\omega t)\bigr),
$$

so

$$
\boxed{\vec{a}(t)=-\omega^2\vec{r}(t)}.
$$

This shows that the acceleration vector is always directed opposite to $\vec{r}(t)$, that is, toward the center of the circle.

Therefore, the acceleration is **centripetal**.

---

#### 6. Visualization of the vectors

- $\vec{r}(t)$ points from the center of the circle to the body
- $\vec{v}(t)$ is tangent to the circle at each point
- $\vec{a}(t)$ points toward the center of the circle

Thus:

- $\vec{r}(t)$ is radial
- $\vec{v}(t)$ is tangential
- $\vec{a}(t)$ is centripetal

Also, $\vec{v}(t)$ is perpendicular to $\vec{r}(t)$, and $\vec{a}(t)$ is opposite to $\vec{r}(t)$.

---

### Final Conclusion

For uniform circular motion of radius $R$ and angular velocity $\omega$,

$$
\boxed{\vec{r}(t)=\bigl(R\cos(\omega t),\,R\sin(\omega t)\bigr)}
$$

$$
\boxed{\vec{v}(t)=\bigl(-R\omega\sin(\omega t),\,R\omega\cos(\omega t)\bigr)}
$$

$$
\boxed{\vec{a}(t)=\bigl(-R\omega^2\cos(\omega t),\,-R\omega^2\sin(\omega t)\bigr)}
$$

and their magnitudes are

$$
\boxed{|\vec{r}(t)|=R, \qquad |\vec{v}(t)|=R\omega, \qquad |\vec{a}(t)|=R\omega^2.}
$$

Since

$$
\boxed{\vec{a}(t)=-\omega^2\vec{r}(t),}
$$

the acceleration is always directed toward the center of the circle. Therefore, the acceleration is **centripetal**.
