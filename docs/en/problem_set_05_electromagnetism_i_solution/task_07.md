# Problem 7 – Motion in a Central Field

## Given

For the central field:

```math
\vec{E}(r)
=
k\frac{Q}{r^2}\hat{r}
```

Find:

1. Equation of motion of the particle.
2. Radial motion case.
3. RK4 numerical method.
4. Positive and negative energy cases.
5. Comparison with gravitational analogy.

Requirement: animation of the motion trajectory.

---

## Solution

A charged particle in an electric field has force:

```math
\vec{F}=q\vec{E}
```

Substitute the given field:

```math
\vec{F}
=
qk\frac{Q}{r^2}\hat{r}
```

Using Newton's second law:

```math
m\vec{a}=\vec{F}
```

Therefore:

```math
m\vec{a}
=
qk\frac{Q}{r^2}\hat{r}
```

So the equation of motion is:

```math
\vec{a}
=
\frac{kqQ}{m r^2}\hat{r}
```

---

## 1. Equation of motion in coordinates

Let:

```math
r=\sqrt{x^2+y^2}
```

and

```math
\hat{r}
=
\frac{(x,y)}{r}
```

Then:

```math
\vec{a}
=
\frac{kqQ}{m r^2}\frac{(x,y)}{r}
```

```math
\vec{a}
=
\frac{kqQ}{m r^3}(x,y)
```

So:

```math
\frac{d^2x}{dt^2}
=
\frac{kqQ}{m}
\frac{x}{(x^2+y^2)^{3/2}}
```

```math
\frac{d^2y}{dt^2}
=
\frac{kqQ}{m}
\frac{y}{(x^2+y^2)^{3/2}}
```

---

## 2. Radial motion

If the particle moves only along the radial direction, then the motion is one-dimensional.

```math
m\frac{d^2r}{dt^2}
=
qk\frac{Q}{r^2}
```

Therefore:

```math
\frac{d^2r}{dt^2}
=
\frac{kqQ}{mr^2}
```

If $qQ>0$, the force is repulsive.  
If $qQ<0$, the force is attractive.

---

## 3. Numerical system for RK4

Introduce variables:

```math
v_x=\frac{dx}{dt}
```

```math
v_y=\frac{dy}{dt}
```

Then the first-order system is:

```math
\frac{dx}{dt}=v_x
```

```math
\frac{dy}{dt}=v_y
```

```math
\frac{dv_x}{dt}
=
\frac{kqQ}{m}
\frac{x}{(x^2+y^2)^{3/2}}
```

```math
\frac{dv_y}{dt}
=
\frac{kqQ}{m}
\frac{y}{(x^2+y^2)^{3/2}}
```

This system can be solved by the RK4 method.

---

## 4. Energy of the particle

Total mechanical energy is:

```math
E_{\text{total}}
=
K+U
```

Kinetic energy:

```math
K
=
\frac{1}{2}m(v_x^2+v_y^2)
```

Potential energy:

```math
U
=
\frac{kqQ}{r}
```

Therefore:

```math
E_{\text{total}}
=
\frac{1}{2}m(v_x^2+v_y^2)
+
\frac{kqQ}{r}
```

For attractive interaction, $qQ<0$:

- negative total energy means bounded motion;
- positive total energy means unbounded motion.

For repulsive interaction, the particle moves away from the center.

---

## 5. Gravitational analogy

The electric central field is similar to the gravitational field because both have inverse-square form.

Electric case:

```math
F_e
=
k\frac{qQ}{r^2}
```

Gravitational case:

```math
F_g
=
G\frac{mM}{r^2}
```

Difference:

- electric force can be attractive or repulsive;
- gravitational force is always attractive;
- electric force depends on charges;
- gravitational force depends on masses.

---

## Final Answer

```math
\vec{a}
=
\frac{kqQ}{m r^2}\hat{r}
```

```math
\frac{d^2x}{dt^2}
=
\frac{kqQ}{m}
\frac{x}{(x^2+y^2)^{3/2}}
```

```math
\frac{d^2y}{dt^2}
=
\frac{kqQ}{m}
\frac{y}{(x^2+y^2)^{3/2}}
```

```math
E_{\text{total}}
=
\frac{1}{2}m(v_x^2+v_y^2)
+
\frac{kqQ}{r}
```

---

## Conclusion

The particle moves in a central inverse-square field.  
If the interaction is attractive, the particle can have bounded motion for negative total energy.  
If the energy is positive, the particle moves away from the center.  
This motion is mathematically similar to motion in a gravitational field.
