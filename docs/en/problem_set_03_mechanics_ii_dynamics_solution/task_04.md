## Problem 4 – Conservation of energy

### Given

A body falls from a height $h$ without air resistance.

We need to:

- write the total energy $E(h)=T(h)+U(h)$,
- determine the velocity as a function of height $v(h)$,
- compare the result with Newton’s second law,
- find the height at which the kinetic energy is equal to 75% of the total energy.

---

## 1. Total mechanical energy

Let the body start from rest at height $h_0$.

The kinetic energy is

$$
T = \frac{1}{2}mv^2
$$

and the gravitational potential energy is

$$
U = mgh
$$

Therefore, the total mechanical energy is

$$
E(h)=T(h)+U(h)=\frac{1}{2}mv(h)^2+mgh
$$

Since there is no air resistance, mechanical energy is conserved:

$$
E = \text{const}
$$

At the initial moment, the body is at height $h_0$ and its velocity is zero, so

$$
E_0 = 0 + mgh_0 = mgh_0
$$

Hence, at any height $h$,

$$
\boxed{
\frac{1}{2}mv(h)^2 + mgh = mgh_0
}
$$

---

## 2. Velocity as a function of height

Starting from energy conservation,

$$
\frac{1}{2}mv(h)^2 + mgh = mgh_0
$$

Move the potential term to the right-hand side:

$$
\frac{1}{2}mv(h)^2 = mg(h_0-h)
$$

Cancel the mass $m$:

$$
\frac{1}{2}v(h)^2 = g(h_0-h)
$$

Multiply both sides by 2:

$$
v(h)^2 = 2g(h_0-h)
$$

Taking the positive square root for the speed, we obtain

$$
\boxed{
v(h)=\sqrt{2g(h_0-h)}
}
$$

This means that the lower the body falls, the greater its speed becomes.

---

## 3. Comparison with Newton’s second law

From Newton’s second law for free fall:

$$
ma = mg
$$

so the acceleration is constant:

$$
a=g
$$

If the body starts from rest and falls a vertical distance

$$
s = h_0 - h
$$

then the kinematic relation gives

$$
v^2 = 2as
$$

Substituting $a=g$ and $s=h_0-h$:

$$
v^2 = 2g(h_0-h)
$$

Thus,

$$
\boxed{
v(h)=\sqrt{2g(h_0-h)}
}
$$

This is exactly the same result as obtained from conservation of energy.  
Therefore, the two methods are fully consistent.

---

## 4. Height at which kinetic energy is 75% of the total energy

We want the kinetic energy to be 75% of the total energy:

$$
T = 0.75E
$$

The total energy is constant and equal to

$$
E = mgh_0
$$

So,

$$
T = 0.75mgh_0
$$

But since

$$
E = T + U
$$

the potential energy must be 25% of the total energy:

$$
U = 0.25E
$$

Using

$$
U = mgh
$$

we get

$$
mgh = 0.25mgh_0
$$

Cancel $mg$:

$$
h = 0.25h_0
$$

Therefore, the kinetic energy is 75% of the total energy when the body is at height

$$
\boxed{
h=\frac{h_0}{4}
}
$$

---

## Final answers

$$
\boxed{
E(h)=\frac{1}{2}mv(h)^2+mgh=mgh_0
}
$$

$$
\boxed{
v(h)=\sqrt{2g(h_0-h)}
}
$$

$$
\boxed{
\text{The result agrees with Newton’s second law}
}
$$

$$
\boxed{
h=\frac{h_0}{4}
}
$$
