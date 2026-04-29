# Problem 4 – Motion of a Particle in a Uniform Field

## Given

The following initial conditions are given:

- $m = 0.02 \ \text{kg}$
- $q = 1 \ \text{mC} = 1 \times 10^{-3} \ \text{C}$
- $\vec{E} = (30,100) \ \text{N/C}$
- $\vec{v}(0) = (20,0) \ \text{m/s}$
- $\vec{r}(0) = (0,0)$

Find:

1. Write the equations of motion and solve them analytically.
2. Draw the motion trajectory.
3. Calculate the time to reach a vertical velocity of $50 \ \text{m/s}$.
4. Calculate the kinetic energy after $t=0.05 \ \text{s}$.
5. Check the consistency with the energy balance.

---

## Solution

Electric force:

```math
\vec{F}=q\vec{E}
```

```math
\vec{F}
=
(1\times10^{-3})(30,100)
=
(0.03,0.1)\ \text{N}
```

Acceleration:

```math
\vec{a}=\frac{\vec{F}}{m}
```

```math
\vec{a}
=
\frac{(0.03,0.1)}{0.02}
=
(1.5,5)\ \text{m/s}^2
```

---

## 1. Equations of motion

Velocity:

```math
\vec{v}(t)=\vec{v}(0)+\vec{a}t
```

```math
v_x(t)=20+1.5t
```

```math
v_y(t)=5t
```

Position:

```math
\vec{r}(t)=\vec{r}(0)+\vec{v}(0)t+\frac{1}{2}\vec{a}t^2
```

```math
x(t)=20t+0.75t^2
```

```math
y(t)=2.5t^2
```

Therefore:

```math
\vec{r}(t)=(20t+0.75t^2,\ 2.5t^2)
```

---

## 2. Motion trajectory

The trajectory is described by:

```math
x(t)=20t+0.75t^2
```

```math
y(t)=2.5t^2
```

The particle moves along a curved path because it has constant acceleration in the electric field.

---

## 3. Time to reach vertical velocity of 50 m/s

```math
v_y(t)=5t
```

```math
50=5t
```

```math
t=10\ \text{s}
```

---

## 4. Kinetic energy after \(t=0.05\) s

At $t=0.05 \ \text{s}$:

```math
v_x=20+1.5(0.05)=20.075\ \text{m/s}
```

```math
v_y=5(0.05)=0.25\ \text{m/s}
```

Kinetic energy:

```math
K=\frac{1}{2}m(v_x^2+v_y^2)
```

```math
K=
\frac{1}{2}(0.02)\left((20.075)^2+(0.25)^2\right)
```

```math
K\approx4.03\ \text{J}
```

---

## 5. Energy balance check

Initial kinetic energy:

```math
K_0=\frac{1}{2}mv_0^2
```

```math
K_0=\frac{1}{2}(0.02)(20)^2
```

```math
K_0=4.00\ \text{J}
```

Position at $t=0.05 \ \text{s}$:

```math
x=20(0.05)+0.75(0.05)^2
```

```math
x=1.001875\ \text{m}
```

```math
y=2.5(0.05)^2
```

```math
y=0.00625\ \text{m}
```

Work done by electric field:

```math
W=q\vec{E}\cdot\vec{r}
```

```math
W=(1\times10^{-3})(30x+100y)
```

```math
W=(1\times10^{-3})(30(1.001875)+100(0.00625))
```

```math
W\approx0.03068\ \text{J}
```

Energy balance:

```math
K=K_0+W
```

```math
K=4.00+0.03068
```

```math
K\approx4.03\ \text{J}
```

So, the energy balance is correct.

---

## Final Answer

```math
\vec{a}=(1.5,5)\ \text{m/s}^2
```

```math
\vec{v}(t)=(20+1.5t,\ 5t)
```

```math
\vec{r}(t)=(20t+0.75t^2,\ 2.5t^2)
```

```math
t=10\ \text{s}
```

```math
K(0.05)\approx4.03\ \text{J}
```

---

## Conclusion

The particle moves with constant acceleration in a uniform electric field.  
The trajectory is curved.  
The kinetic energy increases because the electric field does work on the charged particle.
