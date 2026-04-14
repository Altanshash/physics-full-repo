## Problem 9 – Change of reference frame (Copernican model $\to$ geocentric description)

### Given

Earth and Mars move in circles around the Sun in the same direction.

In the heliocentric reference frame, their position vectors are

$$
\vec{r}_E(t)=R_E(\cos(\omega_E t),\sin(\omega_E t))
$$

$$
\vec{r}_M(t)=R_M(\cos(\omega_M t),\sin(\omega_M t))
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

The position of Earth is

$$
\vec{r}_E(t)=R_E(\cos(\omega_E t),\sin(\omega_E t))
$$

Therefore, its coordinates are

$$
x_E(t)=R_E\cos(\omega_E t)
$$

$$
y_E(t)=R_E\sin(\omega_E t)
$$

So Earth moves uniformly along a circle of radius $R_E$.

The position of Mars is

$$
\vec{r}_M(t)=R_M(\cos(\omega_M t),\sin(\omega_M t))
$$

Therefore, its coordinates are

$$
x_M(t)=R_M\cos(\omega_M t)
$$

$$
y_M(t)=R_M\sin(\omega_M t)
$$

So Mars moves uniformly along a circle of radius $R_M$.

---

#### 2. Position of Mars relative to Earth

The position of Mars relative to Earth is defined by

$$
\vec{r}_{M/E}(t)=\vec{r}_M(t)-\vec{r}_E(t)
$$

Substituting the vectors, we obtain

$$
\vec{r}_{M/E}(t)
=
R_M(\cos(\omega_M t),\sin(\omega_M t))
-
R_E(\cos(\omega_E t),\sin(\omega_E t))
$$

Now subtract the corresponding components:

$$
\vec{r}_{M/E}(t)=
\Bigl(
R_M\cos(\omega_M t)-R_E\cos(\omega_E t),
R_M\sin(\omega_M t)-R_E\sin(\omega_E t)
\Bigr)
$$

Hence,

$$
\boxed{
\vec{r}_{M/E}(t)=
\Bigl(
R_M\cos(\omega_M t)-R_E\cos(\omega_E t),
R_M\sin(\omega_M t)-R_E\sin(\omega_E t)
\Bigr)
}
$$

---

#### 3. Components of the geocentric motion

From the relative position vector, the components are

$$
\boxed{
x_{M/E}(t)=R_M\cos(\omega_M t)-R_E\cos(\omega_E t)
}
$$

$$
\boxed{
y_{M/E}(t)=R_M\sin(\omega_M t)-R_E\sin(\omega_E t)
}
$$

These equations describe the apparent motion of Mars as seen from Earth.

---

#### 4. Geometric interpretation

In the heliocentric frame, both Earth and Mars move on simple circles around the Sun.

However, in the geocentric frame, Mars is described by the relative vector

$$
\vec{r}_{M/E}(t)=\vec{r}_M(t)-\vec{r}_E(t)
$$

This means that the apparent trajectory of Mars is obtained by combining two circular motions:

$$
R_M(\cos(\omega_M t),\sin(\omega_M t))
$$

and

$$
-R_E(\cos(\omega_E t),\sin(\omega_E t))
$$

Therefore, the trajectory of Mars relative to Earth is generally not a circle.

It is a more complicated curve, and this explains why Mars can appear to form loops in the geocentric description.

---

#### 5. Special case

If the angular velocities are equal,

$$
\omega_M=\omega_E=\omega
$$

then

$$
x_{M/E}(t)=R_M\cos(\omega t)-R_E\cos(\omega t)=(R_M-R_E)\cos(\omega t)
$$

$$
y_{M/E}(t)=R_M\sin(\omega t)-R_E\sin(\omega t)=(R_M-R_E)\sin(\omega t)
$$

So in this case

$$
\vec{r}_{M/E}(t)=(R_M-R_E)(\cos(\omega t),\sin(\omega t))
$$

which is again a circle.

Thus, only in this special case does the geocentric trajectory remain circular.

---

### Final Conclusion

In the heliocentric frame,

$$
\vec{r}_E(t)=R_E(\cos(\omega_E t),\sin(\omega_E t))
$$

$$
\vec{r}_M(t)=R_M(\cos(\omega_M t),\sin(\omega_M t))
$$

The position of Mars relative to Earth is

$$
\boxed{
\vec{r}_{M/E}(t)=\vec{r}_M(t)-\vec{r}_E(t)
}
$$

that is,

$$
\boxed{
\vec{r}_{M/E}(t)=
\Bigl(
R_M\cos(\omega_M t)-R_E\cos(\omega_E t),
R_M\sin(\omega_M t)-R_E\sin(\omega_E t)
\Bigr)
}
$$

Therefore, the geocentric coordinates of Mars are

$$
\boxed{
x_{M/E}(t)=R_M\cos(\omega_M t)-R_E\cos(\omega_E t)
}
$$

$$
\boxed{
y_{M/E}(t)=R_M\sin(\omega_M t)-R_E\sin(\omega_E t)
}
$$

So, although Earth and Mars each move on circles around the Sun, the motion of Mars as seen from Earth is generally a more complicated curve rather than a circle.
