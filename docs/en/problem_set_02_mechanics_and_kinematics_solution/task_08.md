## Problem 8 – Relative motion

### Given

Body $A$ moves with velocity

$$
\vec{v}_A=(3,1),
$$

and body $B$ moves with velocity

$$
\vec{v}_B=(1,-2).
$$

Find:

1. Determine the relative velocity $\vec{v}_{A/B}$
2. Determine the direction of the relative motion
3. Visualize the motion of both bodies in:
   - the reference frame attached to the origin of the coordinate system
   - the reference frame attached to body $A$
   - the reference frame attached to body $B$

---

### Solution

#### 1. Relative velocity of body $A$ with respect to body $B$

The relative velocity of $A$ with respect to $B$ is defined as

$$
\vec{v}_{A/B}=\vec{v}_A-\vec{v}_B.
$$

Substitute the given vectors:

$$
\vec{v}_{A/B}=(3,1)-(1,-2).
$$

Compute the components:

$$
\vec{v}_{A/B}=(3-1,\;1-(-2))=(2,3).
$$

Therefore,

$$
\boxed{\vec{v}_{A/B}=(2,3)}.
$$

---

#### 2. Relative velocity of body $B$ with respect to body $A$

Similarly,

$$
\vec{v}_{B/A}=\vec{v}_B-\vec{v}_A.
$$

So,

$$
\vec{v}_{B/A}=(1,-2)-(3,1)=(-2,-3).
$$

Hence,

$$
\boxed{\vec{v}_{B/A}=(-2,-3)}.
$$

This is exactly the opposite of $\vec{v}_{A/B}$, as expected.

---

#### 3. Direction of the relative motion

Since

$$
\vec{v}_{A/B}=(2,3),
$$

the motion of body $A$ relative to body $B$ is directed:

- to the right, because the $x$-component is positive
- upward, because the $y$-component is positive

So the relative motion is along a straight line in the direction of the vector $(2,3)$.

If we want a direction angle $\theta$ measured from the positive $x$-axis, then

$$
\tan\theta=\frac{3}{2}.
$$

Therefore,

$$
\theta=\arctan\left(\frac{3}{2}\right).
$$

So the direction angle is

$$
\boxed{\theta=\arctan\left(\frac{3}{2}\right)}.
$$

This is approximately

$$
\theta \approx 56.3^\circ.
$$

---

#### 4. Motion in the reference frame attached to the origin

In the fixed coordinate system:

- body $A$ moves with constant velocity
  $$
  \vec{v}_A=(3,1)
  $$
- body $B$ moves with constant velocity
  $$
  \vec{v}_B=(1,-2)
  $$

If both bodies start from the origin at $t=0$, then their position vectors are

$$
\vec{r}_A(t)=(3t,t),
$$

$$
\vec{r}_B(t)=(t,-2t).
$$

Thus, in the fixed frame:

- body $A$ moves along the straight line
  $$
  y=\frac{1}{3}x
  $$
- body $B$ moves along the straight line
  $$
  y=-2x
  $$

So both bodies move uniformly along straight lines, but in different directions.

---

#### 5. Motion in the reference frame attached to body $A$

In the frame moving with body $A$, body $A$ is at rest.

Therefore,

$$
\vec{v}_{A/A}=(0,0).
$$

The velocity of body $B$ relative to body $A$ is

$$
\vec{v}_{B/A}=\vec{v}_B-\vec{v}_A=(-2,-3).
$$

So in the frame attached to $A$:

- body $A$ is stationary
- body $B$ moves uniformly with velocity
  $$
  \boxed{\vec{v}_{B/A}=(-2,-3)}
  $$

Thus, body $B$ moves to the left and downward relative to body $A$.

If both bodies coincide at $t=0$, then the relative position of $B$ with respect to $A$ is

$$
\vec{r}_{B/A}(t)=(-2t,-3t).
$$

So body $B$ moves along a straight line through the origin in this frame.

---

#### 6. Motion in the reference frame attached to body $B$

In the frame moving with body $B$, body $B$ is at rest.

Therefore,

$$
\vec{v}_{B/B}=(0,0).
$$

The velocity of body $A$ relative to body $B$ is

$$
\vec{v}_{A/B}=\vec{v}_A-\vec{v}_B=(2,3).
$$

So in the frame attached to $B$:

- body $B$ is stationary
- body $A$ moves uniformly with velocity
  $$
  \boxed{\vec{v}_{A/B}=(2,3)}
  $$

If both bodies coincide at $t=0$, then the relative position of $A$ with respect to $B$ is

$$
\vec{r}_{A/B}(t)=(2t,3t).
$$

Thus, body $A$ moves along a straight line through the origin in the direction $(2,3)$.

---

#### 7. Geometric interpretation

Relative motion shows how one body appears to move when observed from another moving body.

Here:

- in the ground frame, both bodies move with their own constant velocities
- in the frame of body $A$, body $A$ is at rest and body $B$ moves with velocity $(-2,-3)$
- in the frame of body $B$, body $B$ is at rest and body $A$ moves with velocity $(2,3)$

So the relative motion is also uniform rectilinear motion.

---

### Final Conclusion

For the given velocities

$$
\vec{v}_A=(3,1), \qquad \vec{v}_B=(1,-2),
$$

the relative velocity of body $A$ with respect to body $B$ is

$$
\boxed{\vec{v}_{A/B}=(2,3)}
$$

and the relative velocity of body $B$ with respect to body $A$ is

$$
\boxed{\vec{v}_{B/A}=(-2,-3)}.
$$

The relative motion is directed along the vector $(2,3)$, that is, to the right and upward. Its direction angle with the positive $x$-axis is

$$
\boxed{\theta=\arctan\left(\frac{3}{2}\right)\approx 56.3^\circ}.
$$

Thus, in each moving reference frame, one body is at rest and the other moves uniformly along a straight line with the corresponding relative velocity.
