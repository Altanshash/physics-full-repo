# Problem 10 – Angular momentum in circular motion

## Given

Consider circular motion in the $xy$ plane:

$$
\vec r(t) = (R\cos(\omega t),\; R\sin(\omega t),\; 0)
$$

Determine the velocity:

$$
\vec v(t) = \dot{\vec r}(t)
$$

Calculate the angular momentum with respect to the origin:

$$
\vec L(t) = m\,\vec r(t)\times \vec v(t)
$$

Show that

$$
|\vec L| = mR^2\omega
$$

is constant, and that the vector $\vec L$ is perpendicular to the plane of motion.

Interpret the direction of $\vec L$ using the right-hand rule.

(Optional) Add a centripetal force and calculate the torque:

$$
\vec \tau = \vec r \times \vec F
$$

Verify the relation

$$
\vec \tau = \frac{d\vec L}{dt}
$$

for uniform circular motion.

---

## 1. Velocity

Differentiate the position vector:

$$
\vec r(t) = (R\cos(\omega t),\; R\sin(\omega t),\; 0)
$$

Therefore,

$$
\vec v(t) = \dot{\vec r}}(t) = (-R\omega\sin(\omega t),\; R\omega\cos(\omega t),\; 0)
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

Compute the cross product:

$$
\vec r(t)\times\vec v(t)
=
\begin{pmatrix}
0 \\
0 \\
R\cos(\omega t)\cdot R\omega\cos(\omega t)
-
R\sin(\omega t)\cdot(-R\omega\sin(\omega t))
\end{pmatrix}
$$

$$
\vec r(t)\times\vec v(t)
=
\begin{pmatrix}
0 \\
0 \\
R^2\omega\cos^2(\omega t) + R^2\omega\sin^2(\omega t)
\end{pmatrix}
$$

Using

$$
\sin^2(\omega t)+\cos^2(\omega t)=1
$$

we get

$$
\vec r(t)\times\vec v(t) = (0,\;0,\;R^2\omega)
$$

Therefore,

$$
\vec L(t) = (0,\;0,\;mR^2\omega)
$$

---

## 3. Magnitude and direction of angular momentum

The magnitude is

$$
|\vec L| = \sqrt{(mR^2\omega)^2} = mR^2\omega
$$

So $|\vec L|$ is constant.

Also,

$$
\vec L(t) = (0,\;0,\;mR^2\omega)
$$

has only a $z$-component, so it is perpendicular to the $xy$ plane.

Thus, the angular momentum vector is perpendicular to the plane of motion.

---

## 4. Right-hand rule

The motion is counterclockwise in the $xy$ plane.

Using the right-hand rule, curl the fingers of your right hand in the direction of motion. Your thumb points along the positive $z$-axis.

Therefore, $\vec L$ points in the positive $z$ direction.

---

## 5. Torque and the relation $\vec \tau = \frac{d\vec L}{dt}$

For uniform circular motion, the centripetal force is directed toward the origin:

$$
\vec F(t) = -m\omega^2 \vec r(t)
$$

So,

$$
\vec F(t) = (-m\omega^2R\cos(\omega t),\; -m\omega^2R\sin(\omega t),\; 0)
$$

Now compute the torque:

$$
\vec \tau = \vec r \times \vec F
$$

Since $\vec F$ is parallel to $\vec r$, their cross product is zero:

$$
\vec \tau = \vec 0
$$

Now differentiate the angular momentum:

$$
\vec L(t) = (0,\;0,\;mR^2\omega)
$$

Since this vector is constant,

$$
\frac{d\vec L}{dt} = \vec 0
$$

Therefore,

$$
\vec \tau = \frac{d\vec L}{dt}
$$

So the relation is verified.

---

## Final answers

$$
\vec v(t) = (-R\omega\sin(\omega t),\; R\omega\cos(\omega t),\; 0)
$$

$$
\vec L(t) = (0,\;0,\;mR^2\omega)
$$

$$
|\vec L| = mR^2\omega
$$

The vector $\vec L$ is perpendicular to the plane of motion and points in the positive $z$ direction.

$$
\vec \tau = \vec 0
$$

$$
\frac{d\vec L}{dt} = \vec 0
$$

Hence,

$$
\vec \tau = \frac{d\vec L}{dt}
$$
