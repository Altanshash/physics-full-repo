# Problem 8 – Energy of a Three-Charge System

## Given

A system consists of three point charges:

- $q_1$
- $q_2$
- $q_3$

Their positions are:

- $\vec{r}_1$
- $\vec{r}_2$
- $\vec{r}_3$

Find:

1. Total energy of the system
2. Energy for an equilateral triangle configuration
3. Change in energy when the sign of one charge changes
4. Minimum energy configuration numerically
5. Stability of the system

---

## Solution

The potential energy of two point charges is:

```math
U_{ij}
=
k\frac{q_iq_j}{r_{ij}}
```

where:

```math
r_{ij}
=
|\vec{r}_i-\vec{r}_j|
```

For three charges, the total energy is the sum of all pair energies:

```math
U
=
k\left(
\frac{q_1q_2}{r_{12}}
+
\frac{q_1q_3}{r_{13}}
+
\frac{q_2q_3}{r_{23}}
\right)
```

---

## 1. Total energy of the system

```math
U_{\text{total}}
=
U_{12}+U_{13}+U_{23}
```

```math
U_{\text{total}}
=
k\frac{q_1q_2}{r_{12}}
+
k\frac{q_1q_3}{r_{13}}
+
k\frac{q_2q_3}{r_{23}}
```

So:

```math
U_{\text{total}}
=
k\left(
\frac{q_1q_2}{r_{12}}
+
\frac{q_1q_3}{r_{13}}
+
\frac{q_2q_3}{r_{23}}
\right)
```

---

## 2. Equilateral triangle configuration

For an equilateral triangle:

```math
r_{12}=r_{13}=r_{23}=a
```

Then:

```math
U
=
\frac{k}{a}
\left(
q_1q_2+q_1q_3+q_2q_3
\right)
```

If the charges are equal:

```math
q_1=q_2=q_3=q
```

Then:

```math
U
=
\frac{k}{a}
(q^2+q^2+q^2)
```

```math
U
=
\frac{3kq^2}{a}
```

---

## 3. Changing the sign of one charge

If one charge becomes negative:

```math
q_1=q,\quad q_2=q,\quad q_3=-q
```

Then:

```math
U
=
\frac{k}{a}
(q^2-q^2-q^2)
```

```math
U
=
-\frac{kq^2}{a}
```

So the energy changes from:

```math
U_{\text{same signs}}
=
\frac{3kq^2}{a}
```

to:

```math
U_{\text{one negative}}
=
-\frac{kq^2}{a}
```

Energy change:

```math
\Delta U
=
U_{\text{one negative}}-U_{\text{same signs}}
```

```math
\Delta U
=
-\frac{kq^2}{a}
-
\frac{3kq^2}{a}
```

```math
\Delta U
=
-\frac{4kq^2}{a}
```

---

## 4. Minimum energy configuration numerically

To find the minimum energy numerically:

1. Fix two charges to avoid unlimited movement.
2. Move the third charge over a grid.
3. Calculate total energy at each point.
4. Choose the point where the energy is minimum.

Example:

- $q_1=q$
- $q_2=q$
- $q_3=-q$

Fix:

```math
\vec{r}_1=(-1,0)
```

```math
\vec{r}_2=(1,0)
```

Let the third charge move:

```math
\vec{r}_3=(x,y)
```

Then:

```math
U(x,y)
=
k\left(
\frac{q_1q_2}{r_{12}}
+
\frac{q_1q_3}{r_{13}}
+
\frac{q_2q_3}{r_{23}}
\right)
```

The minimum occurs where the negative charge is close to the positive charges.

---

## 5. Stability interpretation

If all charges have the same sign, they repel each other.

Therefore:

- the system has high positive energy;
- charges tend to move apart;
- the configuration is unstable.

If one charge has the opposite sign:

- attractive terms appear;
- the energy becomes lower;
- the system can be more stable, but collapse is possible if charges are allowed to get too close.

---

## Final Answer

```math
U_{\text{total}}
=
k\left(
\frac{q_1q_2}{r_{12}}
+
\frac{q_1q_3}{r_{13}}
+
\frac{q_2q_3}{r_{23}}
\right)
```

For an equilateral triangle:

```math
U
=
\frac{k}{a}
(q_1q_2+q_1q_3+q_2q_3)
```

For three equal positive charges:

```math
U
=
\frac{3kq^2}{a}
```

For two positive charges and one negative charge:

```math
U
=
-\frac{kq^2}{a}
```

Energy change:

```math
\Delta U
=
-\frac{4kq^2}{a}
```

---

## Conclusion

The total energy of a three-charge system is the sum of the three pair interaction energies.  
For equal positive charges, the energy is positive and the system is repulsive.  
When one charge becomes negative, the energy decreases.  
The stability depends on the signs of the charges and their distances.
