# Problem 6 – Two-body Motion and the Barycenter

## Given

We consider two bodies with masses `m1` and `m2`.

Their position vectors are:

- `r1` for body 1
- `r2` for body 2

The barycenter, or center of mass, is:

```text
R = (m1*r1 + m2*r2) / (m1 + m2)
```

For an isolated system:

```text
m1*r1 + m2*r2 = constant
```

The equations of motion are:

```text
m1*r1'' = -G*m1*m2*(r1 - r2) / |r1 - r2|^3
```

```text
m2*r2'' = -G*m1*m2*(r2 - r1) / |r2 - r1|^3
```

---

## Solution

### 1. Center of Mass

The barycenter is defined as:

```text
R = (m1*r1 + m2*r2) / (m1 + m2)
```

This point is the mass-weighted average position of the system.

If `m1 = m2`, the barycenter is exactly between the two bodies.

If `m1 > m2`, the barycenter is closer to body 1.

If `m1 < m2`, the barycenter is closer to body 2.

---

### 2. Isolated System

For an isolated system, there is no external force.

Therefore, the barycenter remains fixed or moves with constant velocity.

If the barycenter is chosen as the origin:

```text
R = 0
```

Then:

```text
m1*r1 + m2*r2 = 0
```

This means both bodies move around their common barycenter.

---

### 3. Equations of Motion

The gravitational force between the two bodies is equal in magnitude and opposite in direction.

For body 1:

```text
m1*r1'' = -G*m1*m2*(r1 - r2) / |r1 - r2|^3
```

For body 2:

```text
m2*r2'' = -G*m1*m2*(r2 - r1) / |r2 - r1|^3
```

The total internal force is:

```text
F1 + F2 = 0
```

Therefore, the barycenter stays fixed in an isolated system.

---

### 4. Dependence on Mass Ratio

The distance of each body from the barycenter depends on the mass ratio.

```text
m1*r1 = m2*r2
```

Therefore:

```text
r1 / r2 = m2 / m1
```

If `m1` is much larger than `m2`, body 1 moves in a small orbit and body 2 moves in a large orbit.

If `m1 = m2`, both bodies move in equal-size orbits around the barycenter.

---

## HTML Requirements

The HTML visualization should include:

- trajectories of both bodies
- marked barycenter
- mass ratio slider

---

## Conclusion

In a two-body gravitational system, both bodies orbit around their common center of mass.

The barycenter is:

```text
R = (m1*r1 + m2*r2) / (m1 + m2)
```

For an isolated system, the barycenter remains fixed or moves uniformly.

The orbit sizes depend on the mass ratio:

```text
r1 / r2 = m2 / m1
```

Thus, when one mass is much larger, the larger body moves only slightly, while the smaller body moves in a much larger orbit.
