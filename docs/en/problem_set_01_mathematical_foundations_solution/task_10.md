# Problem 10 – Angular momentum in circular motion

## Given

Consider circular motion in the $xy$ plane:

$$
\vec r(t) = (R\cos(\omega t),\; R\sin(\omega t),\; 0)
$$

Determine the velocity vector.

$$
\vec v(t) = \dot{\vec r}(t)
$$

Calculate the angular momentum with respect to the origin.

$$
\vec L(t) = m\,\vec r(t)\times\vec v(t)
$$

Show that

$$
|\vec L| = mR^2\omega
$$

is constant, and that $\vec L$ is perpendicular to the plane of motion.

Interpret the direction of $\vec L$ using the right-hand rule.

For the centripetal force, calculate the torque

$$
\vec\tau = \vec r \times \vec F
$$

and verify the relation

$$
\vec\tau = \frac{d\vec L}{dt}
$$

for uniform circular motion.

---

## 1. Velocity vector

Differentiate the position vector:

$$
\vec r(t) = (R\cos(\omega t),\; R\sin(\omega t),\; 0)
$$

Therefore,

$$
\vec v(t) = \dot{\vec r}(t) = (-R\omega\sin(\omega t),\; R\omega\cos(\omega t),\; 0)
$$

---

## 2. Angular momentum

The angular momentum is

$$
\vec L(t) = m\,\vec r(t)\times\vec v(t)
$$

Substitute

$$
\vec r(t) = (R\cos(\omega t),\; R\sin(\omega t),\; 0)
$$

and

$$
\vec v(t) = (-R\omega\sin(\omega t),\; R\omega\cos(\omega t),\; 0)
$$

Since both vectors lie in the $xy$ plane, only the third component of the cross product is nonzero:

$$
\vec r(t)\times\vec v(t) = (0,\; 0,\; xv_y - yv_x)
$$

Here

$$
x = R\cos(\omega t), \qquad y = R\sin(\omega t)
$$

and

$$
v_x = -R\omega\sin(\omega t), \qquad v_y = R\omega\cos(\omega t)
$$

So,

$$
xv_y - yv_x
=
R\cos(\omega t)\cdot R\omega\cos(\omega t)
-
R\sin(\omega t)\cdot\bigl(-R\omega\sin(\omega t)\bigr)
$$

$$
=
R^2\omega\cos^2(\omega t) + R^2\omega\sin^2(\omega t)
$$

$$
=
R^2\omega\bigl(\cos^2(\omega t)+\sin^2(\omega t)\bigr)
$$

$$
=
R^2\omega
$$

Therefore,

$$
\vec r(t)\times\vec v(t) = (0,\; 0,\; R^2\omega)
$$

and hence

$$
\vec L(t) = (0,\; 0,\; mR^2\omega)
$$

---

## 3. Magnitude and direction of $\vec L$

The magnitude is

$$
|\vec L| = \sqrt{(mR^2\omega)^2} = mR^2\omega
$$

So $|\vec L|$ is constant.

Also,

$$
\vec L(t) = (0,\; 0,\; mR^2\omega)
$$

has only a $z$-component, so it is perpendicular to the $xy$ plane.

---

## 4. Right-hand rule

The motion is counterclockwise in the $xy$ plane.

By the right-hand rule, the angular momentum vector points along the positive $z$-axis.

So $\vec L$ points upward, perpendicular to the plane of motion.

---

## 5. Torque and the relation $\vec\tau = \frac{d\vec L}{dt}$

For uniform circular motion, the centripetal force is directed toward the origin:

$$
\vec F(t) = -m\omega^2 \vec r(t)
$$

So,

$$
\vec F(t) = (-m\omega^2R\cos(\omega t),\; -m\omega^2R\sin(\omega t),\; 0)
$$

Now calculate the torque:

$$
\vec\tau = \vec r \times \vec F
$$

Since $\vec F$ is parallel to $\vec r$, their cross product is zero:

$$
\vec\tau = \vec 0
$$

Now differentiate the angular momentum:

$$
\vec L(t) = (0,\; 0,\; mR^2\omega)
$$

Since this is constant,

$$
\frac{d\vec L}{dt} = \vec 0
$$

Therefore,

$$
\vec\tau = \frac{d\vec L}{dt}
$$

So the relation is verified.

---

## Final answers

$$
\vec v(t) = (-R\omega\sin(\omega t),\; R\omega\cos(\omega t),\; 0)
$$

$$
\vec L(t) = (0,\; 0,\; mR^2\omega)
$$

$$
|\vec L| = mR^2\omega
$$

$\vec L$ is perpendicular to the plane of motion and points in the positive $z$ direction.

$$
\vec\tau = \vec 0
$$

$$
\frac{d\vec L}{dt} = \vec 0
$$
