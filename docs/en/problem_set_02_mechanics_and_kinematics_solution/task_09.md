## Problem 9 – Change of reference frame (Copernican model $\to$ geocentric description)

### Given

Earth and Mars move in circles around the Sun in the same direction.

In the heliocentric reference frame, their position vectors are

$$
\vec{r}_E(t)=R_E\bigl(\cos(\omega_E t),\,\sin(\omega_E t)\bigr),
$$

$$
\vec{r}_M(t)=R_M\bigl(\cos(\omega_M t),\,\sin(\omega_M t)\bigr).
$$

Find:

1. Describe both motions in the heliocentric system
2. Determine the position of Mars relative to Earth:
   $$
   \vec{r}_{M/E}(t)=\vec{r}_M(t)-\vec{r}_E(t)
   $$
3. Explicitly write the components $x_{M/E}(t)$ and $y_{M/E}(t)$
4. Interpret the result geometrically

---

### Solution

#### 1. Motion in the heliocentric system

In the heliocentric frame, the Sun is at the origin of coordinates.

The Earth moves on a circle of radius $R_E$ with angular velocity $\omega_E$, so its position vector is

$$
\vec{r}_E(t)=R_E\bigl(\cos(\omega_E t),\,\sin(\omega_E t)\bigr).
$$

Therefore, the components of Earth's motion are

$$
x_E(t)=R_E\cos(\omega_E t),
$$

$$
y_E(t)=R_E\sin(\omega_E t).
$$

Similarly, Mars moves on a circle of radius $R_M$ with angular velocity $\omega_M$, so

$$
\vec{r}_M(t)=R_M\bigl(\cos(\omega_M t),\,\sin(\omega_M t)\bigr).
$$

Its components are

$$
x_M(t)=R_M\cos(\omega_M t),
$$

$$
y_M(t)=R_M\sin(\omega_M t).
$$

Thus, in the heliocentric frame:

- Earth moves uniformly on a circle of radius $R_E$
- Mars moves uniformly on a circle of radius $R_M$

---

#### 2. Position of Mars relative to Earth

To describe Mars as seen from Earth, we subtract Earth's position vector from Mars's position vector:

$$
\vec{r}_{M/E}(t)=\vec{r}_M(t)-\vec{r}_E(t).
$$

Substituting the given vectors:

$$
\vec{r}_{M/E}(t)
=
R_M\bigl(\cos(\omega_M t),\,\sin(\omega_M t)\bigr)
-
R_E\bigl(\cos(\omega_E t),\,\sin(\omega_E t)\bigr).
$$

Now subtract the components:

$$
\vec{r}_{M/E}(t)=
\Bigl(
R_M\cos(\omega_M t)-R_E\cos(\omega_E t),\;
R_M\sin(\omega_M t)-R_E\sin(\omega_E t)
\Bigr).
$$

Therefore,

$$
\boxed{
\vec{r}_{M/E}(t)=
\Bigl(
R_M\cos(\omega_M t)-R_E\cos(\omega_E t),\;
R_M\sin(\omega_M t)-R_E\sin(\omega_E t)
\Bigr)
}.
$$

---

#### 3. Components of the relative motion

From the expression above, the coordinates of Mars relative to Earth are

$$
\boxed{
x_{M/E}(t)=R_M\cos(\omega_M t)-R_E\cos(\omega_E t)
}
$$

and

$$
\boxed{
y_{M/E}(t)=R_M\sin(\omega_M t)-R_E\sin(\omega_E t)
}.
$$

These equations describe the apparent trajectory of Mars in the geocentric reference frame.

---

#### 4. Geometric interpretation

The curve described by

$$
x_{M/E}(t)=R_M\cos(\omega_M t)-R_E\cos(\omega_E t),
$$

$$
y_{M/E}(t)=R_M\sin(\omega_M t)-R_E\sin(\omega_E t),
$$

is generally **not a circle**.

It is the trajectory of Mars as observed from Earth.

This apparent motion is produced by combining two circular motions:

- the real circular motion of Mars around the Sun
- the circular motion of Earth around the Sun

So, even though both planets move in simple circles in the heliocentric system, the motion of Mars relative to Earth becomes more complicated.

This explains why, in the geocentric description, planets can appear to move along loops or retrograde-like paths.

---

#### 5. Special case: equal angular velocities

If

$$
\omega_M=\omega_E=\omega,
$$

then

$$
x_{M/E}(t)=R_M\cos(\omega t)-R_E\cos(\omega t)=(R_M-R_E)\cos(\omega t),
$$

$$
y_{M/E}(t)=R_M\sin(\omega t)-R_E\sin(\omega t)=(R_M-R_E)\sin(\omega t).
$$

Therefore,

$$
\vec{r}_{M/E}(t)=(R_M-R_E)\bigl(\cos(\omega t),\,\sin(\omega t)\bigr),
$$

which is again circular motion.

So, only when the angular velocities are equal does the relative trajectory remain a circle.

---

#### 6. Physical meaning of the change of reference frame

This problem shows the importance of the reference frame.

- In the **heliocentric frame**, both Earth and Mars have simple circular trajectories.
- In the **geocentric frame**, Mars is described by the relative vector
  $$
  \vec{r}_{M/E}(t)=\vec{r}_M(t)-\vec{r}_E(t)
  $$
  and its trajectory becomes more complicated.

Thus, a simple motion in one reference frame may appear much more complex in another reference frame.

---

### Final Conclusion

In the heliocentric system, Earth and Mars move as

$$
\vec{r}_E(t)=R_E\bigl(\cos(\omega_E t),\,\sin(\omega_E t)\bigr),
$$

$$
\vec{r}_M(t)=R_M\bigl(\cos(\omega_M t),\,\sin(\omega_M t)\bigr).
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
R_M\cos(\omega_M t)-R_E\cos(\omega_E t),\;
R_M\sin(\omega_M t)-R_E\sin(\omega_E t)
\Bigr)
}.
$$

Hence, the geocentric components are

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

Therefore, although Earth and Mars each move on circles around the Sun, the trajectory of Mars as seen from Earth is generally a more complicated curve, which explains the geocentric appearance of planetary loops.
