# Problem 3 — Lorentz Transformation

## Given

Two events are given in frame S:

<div align="center">

x₁ = 0 , t₁ = 0

</div>

<br>

<div align="center">

x₂ = 900 m , t₂ = 4 μs

</div>

<br>

Frame S′ moves with velocity:

<div align="center">

v = 0.6c

</div>

<br>

Speed of light:

<div align="center">

c = 3 × 10⁸ m/s

</div>

---

# Solution

## 1. Lorentz Factor

Lorentz factor formula:

<div align="center">

γ = 1 / √(1 − v²/c²)

</div>

<br>

Substitute the velocity:

<div align="center">

γ = 1 / √(1 − 0.6²)

</div>

<br>

<div align="center">

γ = 1 / √(1 − 0.36)

</div>

<br>

<div align="center">

γ = 1 / √0.64

</div>

<br>

<div align="center">

γ = 1 / 0.8

</div>

<br>

<div align="center">

γ = 1.25

</div>

---

# 2. Transform the Position Coordinate

Position transformation formula:

<div align="center">

x′ = γ(x − vt)

</div>

<br>

Given:

<div align="center">

x = 900 m

</div>

<br>

<div align="center">

t = 4 × 10⁻⁶ s

</div>

<br>

Velocity:

<div align="center">

v = 0.6 × 3 × 10⁸

</div>

<br>

<div align="center">

v = 1.8 × 10⁸ m/s

</div>

<br>

First calculate vt:

<div align="center">

vt = (1.8 × 10⁸)(4 × 10⁻⁶)

</div>

<br>

<div align="center">

vt = 720 m

</div>

<br>

Now substitute:

<div align="center">

x′ = 1.25(900 − 720)

</div>

<br>

<div align="center">

x′ = 1.25(180)

</div>

<br>

<div align="center">

x′ = 225 m

</div>

---

# 3. Transform the Time Coordinate

Time transformation formula:

<div align="center">

t′ = γ(t − vx/c²)

</div>

<br>

First calculate vx:

<div align="center">

vx = (1.8 × 10⁸)(900)

</div>

<br>

<div align="center">

vx = 1.62 × 10¹¹

</div>

<br>

Calculate c²:

<div align="center">

c² = (3 × 10⁸)²

</div>

<br>

<div align="center">

c² = 9 × 10¹⁶

</div>

<br>

Now calculate:

<div align="center">

vx/c² = (1.62 × 10¹¹) / (9 × 10¹⁶)

</div>

<br>

<div align="center">

vx/c² = 1.8 × 10⁻⁶ s

</div>

<br>

Substitute into the formula:

<div align="center">

t′ = 1.25(4 × 10⁻⁶ − 1.8 × 10⁻⁶)

</div>

<br>

<div align="center">

t′ = 1.25(2.2 × 10⁻⁶)

</div>

<br>

<div align="center">

t′ = 2.75 × 10⁻⁶ s

</div>

<br>

<div align="center">

t′ = 2.75 μs

</div>

---

# 4. Can the Order of Events Change?

First event:

<div align="center">

t₁′ = 0

</div>

<br>

Second event:

<div align="center">

t₂′ = 2.75 μs

</div>

<br>

Since:

<div align="center">

t₂′ > t₁′

</div>

<br>

the order of events does not change.

Now calculate:

<div align="center">

cΔt = (3 × 10⁸)(4 × 10⁻⁶)

</div>

<br>

<div align="center">

cΔt = 1200 m

</div>

<br>

Spatial separation:

<div align="center">

Δx = 900 m

</div>

<br>

Since:

<div align="center">

cΔt > Δx

</div>

<br>

the interval is timelike.

Therefore, the order of events cannot change in any inertial frame.

---

# 5. Spacetime Interval

Spacetime interval formula:

<div align="center">

s² = c²t² − x²

</div>

<br>

This can also be written as:

<div align="center">

s² = (ct)² − x²

</div>

<br>

Calculate ct:

<div align="center">

ct = (3 × 10⁸)(4 × 10⁻⁶)

</div>

<br>

<div align="center">

ct = 1200 m

</div>

<br>

Now calculate:

<div align="center">

s² = 1200² − 900²

</div>

<br>

<div align="center">

s² = 1,440,000 − 810,000

</div>

<br>

<div align="center">

s² = 630,000 m²

</div>

---

# 6. Verify Invariance

In frame S′:

<div align="center">

x′ = 225 m

</div>

<br>

<div align="center">

t′ = 2.75 × 10⁻⁶ s

</div>

<br>

Calculate ct′:

<div align="center">

ct′ = (3 × 10⁸)(2.75 × 10⁻⁶)

</div>

<br>

<div align="center">

ct′ = 825 m

</div>

<br>

Now calculate:

<div align="center">

s′² = 825² − 225²

</div>

<br>

<div align="center">

s′² = 680,625 − 50,625

</div>

<br>

<div align="center">

s′² = 630,000 m²

</div>

<br>

Therefore:

<div align="center">

s′² = s²

</div>

---

# Conclusion

The transformed coordinates of the second event in frame S′ are:

<div align="center">

x₂′ = 225 m

</div>

<br>

<div align="center">

t₂′ = 2.75 μs

</div>

<br>

The order of events does not change because the interval is timelike.

The spacetime interval is:

<div align="center">

s² = 630,000 m²

</div>

<br>

The interval is the same in both frames:

<div align="center">

s′² = s²

</div>

<br>

Thus, the spacetime interval is invariant under Lorentz transformation.
