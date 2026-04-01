## Problem 2 – Inclined plane with friction

### Given

A body of mass $m$ slides down an inclined plane with angle $\alpha$.  
The coefficient of kinetic friction is $\mu$.

We need to:

- determine all forces acting on the body,
- derive the acceleration,
- calculate the time of descent from height $h$,
- determine the final velocity,
- check the consistency with the energy balance.

---

## 1. Forces acting on the body

Three forces act on the body:

1. **Gravitational force**
   $$
   \vec{F}_g = m\vec{g}
   $$

2. **Normal force**
   $$
   \vec{N}
   $$
   perpendicular to the plane.

3. **Kinetic friction**
   $$
   \vec{F}_f
   $$
   directed opposite to the motion along the plane.

---

## 2. Components of gravity

We decompose the gravitational force into components parallel and perpendicular to the plane.

The component along the plane is

$$
F_{\parallel} = mg \sin\alpha
$$

The component perpendicular to the plane is

$$
F_{\perp} = mg \cos\alpha
$$

Since the body does not move perpendicular to the surface, the normal force is

$$
N = mg \cos\alpha
$$

The kinetic friction force has magnitude

$$
F_f = \mu N = \mu mg \cos\alpha
$$

Because friction acts upward along the plane, the net force along the plane is

$$
F_{\text{net}} = mg\sin\alpha - \mu mg\cos\alpha
$$

---

## 3. Acceleration

Apply Newton’s second law along the plane:

$$
ma = mg\sin\alpha - \mu mg\cos\alpha
$$

Divide both sides by $m$:

$$
a = g\sin\alpha - \mu g\cos\alpha
$$

Therefore,

$$
\boxed{a = g(\sin\alpha - \mu\cos\alpha)}
$$

For the body to slide downward, we need

$$
\sin\alpha > \mu\cos\alpha
$$

---

## 4. Time of descent from height $h$

Let $h$ be the vertical height of the incline.  
Then the distance traveled along the plane is

$$
s = \frac{h}{\sin\alpha}
$$

Assume the body starts from rest, so

$$
v_0 = 0
$$

Using the kinematic formula

$$
s = \frac{1}{2}at^2
$$

we get

$$
\frac{h}{\sin\alpha} = \frac{1}{2}at^2
$$

Substitute the expression for acceleration:

$$
\frac{h}{\sin\alpha}
=
\frac{1}{2}g(\sin\alpha - \mu\cos\alpha)t^2
$$

Now solve for $t^2$:

$$
t^2
=
\frac{2h}{g\sin\alpha(\sin\alpha - \mu\cos\alpha)}
$$

Hence, the descent time is

$$
\boxed{
t =
\sqrt{
\frac{2h}{g\sin\alpha(\sin\alpha - \mu\cos\alpha)}
}
}
$$

---

## 5. Final velocity

Use the relation

$$
v^2 = v_0^2 + 2as
$$

Since the body starts from rest, $v_0=0$, so

$$
v^2 = 2as
$$

Substitute

$$
a = g(\sin\alpha - \mu\cos\alpha),
\qquad
s = \frac{h}{\sin\alpha}
$$

Then

$$
v^2
=
2g(\sin\alpha - \mu\cos\alpha)\frac{h}{\sin\alpha}
$$

Therefore,

$$
v^2
=
\frac{2gh(\sin\alpha - \mu\cos\alpha)}{\sin\alpha}
$$

and the final velocity is

$$
\boxed{
v =
\sqrt{
\frac{2gh(\sin\alpha - \mu\cos\alpha)}{\sin\alpha}
}
}
$$

---

## 6. Energy balance check

Initially, the body has gravitational potential energy

$$
E_p = mgh
$$

At the bottom, this energy is converted into kinetic energy and work against friction.

The work done by friction is

$$
W_f = -F_f s
$$

Substitute

$$
F_f = \mu mg\cos\alpha,
\qquad
s = \frac{h}{\sin\alpha}
$$

Then

$$
W_f
=
-\mu mg\cos\alpha \cdot \frac{h}{\sin\alpha}
$$

The energy equation is

$$
mgh + W_f = \frac{1}{2}mv^2
$$

So,

$$
mgh - \mu mg\cos\alpha \cdot \frac{h}{\sin\alpha}
=
\frac{1}{2}mv^2
$$

Factor out $mgh$ on the left:

$$
mgh\left(1 - \mu\frac{\cos\alpha}{\sin\alpha}\right)
=
\frac{1}{2}mv^2
$$

Multiply both sides by $\frac{2}{m}$:

$$
2gh\left(1 - \mu\frac{\cos\alpha}{\sin\alpha}\right)
=
v^2
$$

Rewrite the expression:

$$
v^2
=
\frac{2gh(\sin\alpha - \mu\cos\alpha)}{\sin\alpha}
$$

This is exactly the same result as obtained from kinematics.  
Therefore, the result is consistent with the energy balance.

---

## Final answers

$$
\boxed{N = mg\cos\alpha}
$$

$$
\boxed{F_f = \mu mg\cos\alpha}
$$

$$
\boxed{a = g(\sin\alpha - \mu\cos\alpha)}
$$

$$
\boxed{
t =
\sqrt{
\frac{2h}{g\sin\alpha(\sin\alpha - \mu\cos\alpha)}
}
}
$$

$$
\boxed{
v =
\sqrt{
\frac{2gh(\sin\alpha - \mu\cos\alpha)}{\sin\alpha}
}
}
$$
