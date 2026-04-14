## Problem 9 – Change of reference frame (Copernican model to geocentric description)

### Given

Earth and Mars move in circles around the Sun in the same direction.

In the heliocentric reference frame, their position vectors are

$$
\vec{r}_E(t) = \left( R_E \cos(\omega_E t),\ R_E \sin(\omega_E t) \right)
$$

$$
\vec{r}_M(t) = \left( R_M \cos(\omega_M t),\ R_M \sin(\omega_M t) \right)
$$

Find:

1. Describe both motions in the heliocentric system
2. Determine the position of Mars relative to Earth
3. Write explicitly the components $x_{M/E}(t)$ and $y_{M/E}(t)$
4. Explain the geometric meaning of the result

---

### Solution

#### 1. Motion in the heliocentric system

In the heliocentric frame, the Sun is at the origin.

The position vector of Earth is

$$
\vec{r}_E(t) = \left( R_E \cos(\omega_E t),\ R_E \sin(\omega_E t) \right)
$$

So its coordinates are

$$
x_E(t) = R_E \cos(\omega_E t)
$$

$$
y_E(t) = R_E \sin(\omega_E t)
$$

Thus, Earth moves uniformly along a circle of radius $R_E$.

The position vector of Mars is

$$
\vec{r}_M(t) = \left( R_M \cos(\omega_M t),\ R_M \sin(\omega_M t) \right)
$$

So its coordinates are

$$
x_M(t) = R_M \cos(\omega_M t)
$$

$$
y_M(t) = R_M \sin(\omega_M t)
$$

Thus, Mars moves uniformly along a circle of radius $R_M$.

---

#### 2. Position of Mars relative to Earth

The position of Mars relative to Earth is defined by

$$
\vec{r}_{M/E}(t) = \vec{r}_M(t) - \vec{r}_E(t)
$$

Substituting the vectors, we get

$$
\vec{r}_{M/E}(t) = \left( R_M \cos(\omega_M t),\ R_M \sin(\omega_M t) \right) - \left( R_E \cos(\omega_E t),\ R_E \sin(\omega_E t) \right)
$$

Now subtract the corresponding components:

$$
\vec{r}_{M/E}(t) = \left( R_M \cos(\omega_M t) - R_E \cos(\omega_E t),\ R_M \sin(\omega_M t) - R_E \sin(\omega_E t) \right)
$$

Therefore,

$$
\boxed{\vec{r}_{M/E}(t) = \left( R_M \cos(\omega_M t) - R_E \cos(\omega_E t),\ R_M \sin(\omega_M t) - R_E \sin(\omega_E t) \right)}
$$

---

#### 3. Components of the geocentric motion

From the relative position vector, the components are

$$
\boxed{x_{M/E}(t) = R_M \cos(\omega_M t) - R_E \cos(\omega_E t)}
$$

$$
\boxed{y_{M/E}(t) = R_M \sin(\omega_M t) - R_E \sin(\omega_E t)}
$$

These equations describe the apparent motion of Mars as seen from Earth.

---

#### 4. Geometric interpretation

In the heliocentric frame, both Earth and Mars move on circles around the Sun.

In the geocentric frame, Mars is described by the relative vector

$$
\vec{r}_{M/E}(t) = \vec{r}_M(t) - \vec{r}_E(t)
$$

Therefore, the motion of Mars as seen from Earth is obtained by combining two circular motions.

In general, this trajectory is not a circle. It is a more complicated curve, which explains why Mars may appear to form loops in the geocentric description.

---

#### 5. Special case

If the angular velocities are equal,

$$
\omega_M = \omega_E = \omega
$$

then

$$
x_{M/E}(t) = R_M \cos(\omega t) - R_E \cos(\omega t) = (R_M - R_E)\cos(\omega t)
$$

$$
y_{M/E}(t) = R_M \sin(\omega t) - R_E \sin(\omega t) = (R_M - R_E)\sin(\omega t)
$$

So in this case

$$
\vec{r}_{M/E}(t) = \left( (R_M - R_E)\cos(\omega t),\ (R_M - R_E)\sin(\omega t) \right)
$$

which is again a circle.

---

### Final Conclusion

In the heliocentric frame,

$$
\vec{r}_E(t) = \left( R_E \cos(\omega_E t),\ R_E \sin(\omega_E t) \right)
$$

$$
\vec{r}_M(t) = \left( R_M \cos(\omega_M t),\ R_M \sin(\omega_M t) \right)
$$

The position of Mars relative to Earth is

$$
\boxed{\vec{r}_{M/E}(t) = \vec{r}_M(t) - \vec{r}_E(t)}
$$

that is,

$$
\boxed{\vec{r}_{M/E}(t) = \left( R_M \cos(\omega_M t) - R_E \cos(\omega_E t),\ R_M \sin(\omega_M t) - R_E \sin(\omega_E t) \right)}
$$

Therefore, the geocentric coordinates of Mars are

$$
\boxed{x_{M/E}(t) = R_M \cos(\omega_M t) - R_E \cos(\omega_E t)}
$$

$$
\boxed{y_{M/E}(t) = R_M \sin(\omega_M t) - R_E \sin(\omega_E t)}
$$

So, although Earth and Mars each move on circles around the Sun, the motion of Mars as seen from Earth is generally a more complicated curve.
