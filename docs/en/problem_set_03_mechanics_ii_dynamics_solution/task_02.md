## Problem 2 – Inclined plane with friction

### Given

A body of mass $m$ slides down an inclined plane with angle $\alpha$.  
The coefficient of kinetic friction is $\mu$.

We need to:

- determine all forces acting on the body,
- derive the acceleration $\vec{a}$,
- calculate the time of descent from height $h$,
- determine the final velocity $\vec{v}$,
- check the consistency with the energy balance.

---

## 1. Forces acting on the body

Three forces act on the body:

1. **Gravity**

$$
\vec{F}_g = m\vec{g}
$$

It acts vertically downward.

2. **Normal force**

$$
\vec{N}
$$

It acts perpendicular to the plane.

3. **Kinetic friction**

$$
\vec{F}_f
$$

It acts along the plane, opposite to the direction of motion.

---

## 2. Decomposition of gravity

Resolve the gravitational force into components relative to the plane.

The component parallel to the plane is

$$
F_{\parallel} = mg \sin\alpha
$$

The component perpendicular to the plane is

$$
F_{\perp} = mg \cos\alpha
$$

Since there is no motion perpendicular to the plane, the normal force is

$$
N = mg \cos\alpha
$$

The kinetic friction force is

$$
F_f = \mu N = \mu mg \cos\alpha
$$

Because friction acts up the plane, the net force along the plane is

$$
F_{\text{net}} = mg \sin\alpha - \mu mg \cos\alpha
$$

---

## 3. Acceleration

Using Newton’s second law along the plane:

$$
ma = mg \sin\alpha - \mu mg \cos\alpha
$$

Divide both sides by $m$:

$$
a = g \sin\alpha - \mu g \cos\alpha
$$

Thus, the acceleration is

$$
\boxed{a = g(\sin\alpha - \mu \cos\alpha)}
$$

The body moves downward only if

$$
\sin\alpha > \mu \cos\alpha
$$

---

## 4. Time of descent from height $h$

If the vertical height of the incline is $h$, then the distance traveled along the plane is

$$
s = \frac{h}{\sin\alpha}
$$

Assume the body starts from rest, so

$$
v_0 = 0
$$

Using the kinematic relation

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
\frac{1}{2}g(\sin\alpha - \mu \cos\alpha)t^2
$$

Solve for $t^2$:

$$
t^2
=
\frac{2h}{g \sin\alpha \, (\sin\alpha - \mu \cos\alpha)}
$$

Therefore, the descent time is

$$
\boxed{
t =
\sqrt{
\frac{2h}{g \sin\alpha \, (\sin\alpha - \mu \cos\alpha)}
}
}
$$

---

## 5. Final velocity

Use the formula

$$
v^2 = v_0^2 + 2as
$$

Since $v_0 = 0$, we have

$$
v^2 = 2as
$$

Substitute

$$
a = g(\sin\alpha - \mu \cos\alpha),
\qquad
s = \frac{h}{\sin\alpha}
$$

Then

$$
v^2
=
2g(\sin\alpha - \mu \cos\alpha)\frac{h}{\sin\alpha}
$$

So the final velocity is

$$
\boxed{
v =
\sqrt{
\frac{2gh(\sin\alpha - \mu \cos\alpha)}{\sin\alpha}
}
}
$$

---

## 6. Energy balance check

Initially, the body has gravitational potential energy

$$
E_p = mgh
$$

As it slides down, part of this energy becomes kinetic energy, and part is lost to friction.

The work done by friction is

$$
W_f = -F_f s
$$

Substitute

$$
F_f = \mu mg \cos\alpha,
\qquad
s = \frac{h}{\sin\alpha}
$$

Thus,

$$
W_f
=
-\mu mg \cos\alpha \cdot \frac{h}{\sin\alpha}
$$

The energy balance is

$$
mgh + W_f = \frac{1}{2}mv^2
$$

So,

$$
mgh - \mu mg \cos\alpha \cdot \frac{h}{\sin\alpha}
=
\frac{1}{2}mv^2
$$

Factor out $mgh$:

$$
mgh
\left(
1 - \mu \frac{\cos\alpha}{\sin\alpha}
\right)
=
\frac{1}{2}mv^2
$$

Multiply both sides by $\frac{2}{m}$:

$$
2gh
\left(
1 - \mu \frac{\cos\alpha}{\sin\alpha}
\right)
=
v^2
$$

Rewrite the expression:

$$
v^2
=
\frac{2gh(\sin\alpha - \mu \cos\alpha)}{\sin\alpha}
$$

This is exactly the same result as obtained from kinematics.

So the result is consistent with the energy balance.

---

## Final answers

$$
N = mg \cos\alpha
$$

$$
F_f = \mu mg \cos\alpha
$$

$$
\boxed{a = g(\sin\alpha - \mu \cos\alpha)}
$$

$$
\boxed{
t =
\sqrt{
\frac{2h}{g \sin\alpha \, (\sin\alpha - \mu \cos\alpha)}
}
}
$$

$$
\boxed{
v =
\sqrt{
\frac{2gh(\sin\alpha - \mu \cos\alpha)}{\sin\alpha}
}
}
$$
