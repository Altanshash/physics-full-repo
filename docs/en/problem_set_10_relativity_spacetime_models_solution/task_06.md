# Problem 6 — Minkowski Diagram

## Given

Implement the Lorentz transformation as a matrix.

Draw the following axes:

<div align="center">

ct and x axes

</div>

<br>

<div align="center">

ct′ and x′ axes

</div>

<br>

Mark the light cone.

Allow velocity change with a slider.

Geometrically interpret:

<div align="center">

time dilation and length contraction

</div>

---

# Solution

## 1. Lorentz Transformation as a Matrix

Let:

<div align="center">

β = v / c

</div>

<br>

The Lorentz factor is:

<div align="center">

γ = 1 / √(1 − β²)

</div>

<br>

The Lorentz transformation is:

<div align="center">

ct′ = γ(ct − βx)

</div>

<br>

<div align="center">

x′ = γ(x − βct)

</div>

<br>

In matrix form:

<div align="center">

[ ct′ ] = [ γ&nbsp;&nbsp;&nbsp;−βγ ] [ ct ]

</div>

<div align="center">

[ x′  ] = [ −βγ&nbsp;&nbsp;&nbsp;γ ] [ x ]

</div>

---

## 2. Draw the ct and x Axes

In a Minkowski diagram, the horizontal axis represents position:

<div align="center">

x

</div>

<br>

The vertical axis represents time multiplied by the speed of light:

<div align="center">

ct

</div>

<br>

The stationary frame S has perpendicular axes:

<div align="center">

x-axis: horizontal

</div>

<br>

<div align="center">

ct-axis: vertical

</div>

---

## 3. Draw the ct′ and x′ Axes

For the moving frame S′, the axes are tilted.

The ct′ axis is the path of the moving origin:

<div align="center">

x = vt

</div>

<br>

Using β:

<div align="center">

x = βct

</div>

<br>

The x′ axis represents events that occur at:

<div align="center">

t′ = 0

</div>

<br>

From the Lorentz transformation:

<div align="center">

ct′ = γ(ct − βx)

</div>

<br>

If:

<div align="center">

ct′ = 0

</div>

<br>

then:

<div align="center">

ct = βx

</div>

<br>

So the moving axes are:

<div align="center">

ct′ axis: x = βct

</div>

<br>

<div align="center">

x′ axis: ct = βx

</div>

---

## 4. Mark the Light Cone

Light travels with speed:

<div align="center">

c

</div>

<br>

Therefore:

<div align="center">

x = ct

</div>

<br>

and:

<div align="center">

x = −ct

</div>

<br>

These two lines form the light cone.

In the diagram, the light cone is drawn as two diagonal lines:

<div align="center">

45° upward and 45° downward

</div>

<br>

The light cone is invariant under Lorentz transformations.

---

## 5. Allow Velocity Change with a Slider

The slider changes the value of β:

<div align="center">

0 ≤ β < 1

</div>

<br>

When β increases, the Lorentz factor increases:

<div align="center">

γ = 1 / √(1 − β²)

</div>

<br>

As β approaches 1:

<div align="center">

γ → ∞

</div>

<br>

The ct′ and x′ axes move closer to the light cone.

---

## 6. Geometrical Interpretation

## Time Dilation

Time dilation means that a moving clock ticks more slowly.

In the Minkowski diagram, this appears because the ct′ axis is tilted toward the light cone.

The relation is:

<div align="center">

Δt = γΔt₀

</div>

<br>

Since:

<div align="center">

γ > 1

</div>

<br>

the time measured in the stationary frame is greater than the proper time.

---

## Length Contraction

Length contraction means that a moving object appears shorter in the direction of motion.

The relation is:

<div align="center">

L = L₀ / γ

</div>

<br>

Since:

<div align="center">

γ > 1

</div>

<br>

the measured length is smaller than the proper length.

In the Minkowski diagram, length contraction is connected to measuring both ends of an object at the same time in one reference frame.

This depends on the tilted x′ axis and the relativity of simultaneity.

---

# Conclusion

A Minkowski diagram shows the geometry of special relativity.

The stationary frame S uses the axes:

<div align="center">

ct and x

</div>

<br>

The moving frame S′ uses the tilted axes:

<div align="center">

ct′ and x′

</div>

<br>

The light cone remains fixed because the speed of light is the same for all inertial observers.

As velocity increases:

<div align="center">

β → 1

</div>

<br>

the Lorentz factor increases:

<div align="center">

γ → ∞

</div>

<br>

and the moving axes approach the light cone.

This diagram gives a geometric explanation of time dilation, length contraction, and the invariance of the speed of light.
