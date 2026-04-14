# Problem 10 – Angular momentum in circular motion

## Given

Consider circular motion in the $xy$ plane:

$$
\vec r(t) = (R\cos(\omega t),\; R\sin(\omega t),\; 0)
$$

We need to:

1. determine the velocity
   $$
   \vec v(t) = \dot{\vec r}(t),
   $$
2. calculate the angular momentum with respect to the origin
   $$
   \vec L(t) = m\,\vec r(t)\times \vec v(t),
   $$
3. show that $|\vec L| = mR^2\omega$ is constant, and that $\vec L$ is perpendicular to the plane of motion,
4. interpret the direction of $\vec L$ using the right-hand rule,
5. optionally, add a constant centripetal force and calculate the torque
   $$
   \vec \tau = \vec r \times \vec F
   $$
   and verify the relation
   $$
   \vec \tau = \frac{d\vec L}{dt}
   $$
   for uniform circular motion.

---

## 1. Velocity

Differentiate the position vector componentwise:

$$
\vec r(t) = (R\cos(\omega t),\; R\sin(\omega t),\; 0)
$$

Therefore,

$$
\vec v(t) = \dot{\vec r}(t)
= (-R\omega\sin(\omega t),\; R\omega\cos(\omega t),\; 0)
$$

---

## 2. Angular momentum

The angular momentum is

$$
\vec L(t) = m\,\vec r(t)\times \vec v(t)
$$

Substitute $\vec r(t)$ and $\vec v(t)$:

$$
\vec r(t) = (R\cos(\omega t),\; R\sin(\omega t),\; 0)
$$

$$
\vec v(t) = (-R\omega\sin(\omega t),\; R\omega\cos(\omega t),\; 0)
$$

Now compute the cross product.

Since both vectors lie in the $xy$ plane, only the $z$ component is nonzero:

$$
\vec r(t)\times \vec v(t)
=
\left(0,\;0,\;xv_y - yv_x\right)
$$

Here,

$$
x = R\cos(\omega t), \qquad y = R\sin(\omega t)
$$

$$
v_x = -R\omega\sin(\omega t), \qquad v_y = R\omega\cos(\omega t)
$$

So,

$$
xv_y - yv_x
=
R\cos(\omega t)\cdot R\omega\cos(\omega t)
-
R\sin(\omega t)\cdot\left(-R\omega\sin(\omega t)\right)
$$

$$
=
R^2\omega\cos^2(\omega t) + R^2\omega\sin^2(\omega t)
$$

$$
=
R^2\omega\left(\cos^2(\omega t)+\sin^2(\omega t)\right)
$$

$$
=
R^2\omega
$$

Hence,

$$
\vec r(t)\times \vec v(t) = (0,\;0,\;R^2\omega)
$$

Therefore,

$$
\vec L(t) = m(0,\;0,\;R^2\omega)
$$

So,

$$
\vec L(t) = (0,\;0,\;mR^2\omega)
$$

---

## 3. Magnitude and direction of $\vec L$

The magnitude is

$$
|\vec L| = \sqrt{0^2 + 0^2 + (mR^2\omega)^2}
$$

$$
|\vec L| = mR^2\omega
$$

This is constant because $m$, $R$, and $\omega$ are constant.

Also, the vector

$$
\vec L = (0,\;0,\;mR^2\omega)
$$

has only a $z$ component, so it is perpendicular to the $xy$ plane of motion.

Thus:

$$
|\vec L| = mR^2\omega = \text{constant}
$$

and $\vec L$ is perpendicular to the plane of motion.

---

## 4. Right-hand rule

The particle moves counterclockwise in the $xy$ plane when viewed from above, because

$$
\vec r(t) = (R\cos(\omega t),\; R\sin(\omega t),\; 0)
$$

Using the right-hand rule, curl the fingers of the right hand in the direction of motion. Then the thumb points in the direction of $\vec L$.

Therefore, $\vec L$ points along the positive $z$ axis.

So the direction of angular momentum is

$$
\vec L \parallel \hat{k}
$$

---

## 5. Torque and the relation $\vec\tau = \frac{d\vec L}{dt}$

For uniform circular motion, the centripetal force points toward the center:

$$
\vec F(t) = -m\omega^2 \vec r(t)
$$

Thus,

$$
\vec F(t) = (-m\omega^2 R\cos(\omega t),\; -m\omega^2 R\sin(\omega t),\; 0)
$$

Now compute the torque:

$$
\vec \tau = \vec r \times \vec F
$$

Since $\vec F$ is parallel to $\vec r$, their cross product is zero:

$$
\vec \tau = \vec 0
$$

Now differentiate $\vec L$:

$$
\vec L = (0,\;0,\;mR^2\omega)
$$

Since this is constant,

$$
\frac{d\vec L}{dt} = \vec 0
$$

Therefore,

$$
\vec \tau = \frac{d\vec L}{dt} = \vec 0
$$

So the relation is verified for uniform circular motion.

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

$\vec L$ is perpendicular to the plane of motion and points along the positive $z$ axis.

For the centripetal force,

$$
\vec F(t) = -m\omega^2\vec r(t)
$$

the torque is

$$
\vec \tau = \vec 0
$$

and

$$
\frac{d\vec L}{dt} = \vec 0
$$

so

$$
\vec \tau = \frac{d\vec L}{dt}
$$
