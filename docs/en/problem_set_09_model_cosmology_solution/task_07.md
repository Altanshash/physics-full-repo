# Problem 7 – Newton's Gravity and Orbit Classification

## Given

Motion occurs in a central gravitational field.

The gravitational force is:

$$F=-\frac{GMm}{r^2}$$

The total mechanical energy is:

$$E=\frac{1}{2}mv^2-\frac{GMm}{r}$$

Where:

- $G$ is the gravitational constant.
- $M$ is the central mass.
- $m$ is the orbiting mass.
- $r$ is the distance from the center.
- $v$ is the speed of the orbiting body.
- $E$ is the total energy.

---

## Solution

### 1. Orbit Classification by Energy

The type of orbit depends on the sign of the total energy.

If:

$$E<0$$

then the orbit is bound. This means the body cannot escape the gravitational field.

This case gives an elliptical orbit.

If:

$$E=0$$

then the body is exactly at escape energy.

This case gives a parabolic trajectory.

If:

$$E>0$$

then the body has enough energy to escape.

This case gives a hyperbolic trajectory.

---

### 2. Initial Conditions

The total energy is:

$$E=\frac{1}{2}mv^2-\frac{GMm}{r}$$

For a fixed initial distance $r$, the orbit type depends mainly on the initial velocity $v$.

The escape velocity is found by setting:

$$E=0$$

So:

$$\frac{1}{2}mv^2=\frac{GMm}{r}$$

Solving for $v$:

$$v=\sqrt{\frac{2GM}{r}}$$

This is the escape velocity.

If:

$$v<\sqrt{\frac{2GM}{r}}$$

then:

$$E<0$$

and the orbit is bound.

If:

$$v=\sqrt{\frac{2GM}{r}}$$

then:

$$E=0$$

and the trajectory is parabolic.

If:

$$v>\sqrt{\frac{2GM}{r}}$$

then:

$$E>0$$

and the trajectory is hyperbolic.

---

### 3. Numerical Investigation

In the simulation, the body starts at a chosen distance from the central mass.

The initial velocity can be changed using a slider.

For each velocity, the program calculates:

$$E=\frac{1}{2}mv^2-\frac{GMm}{r}$$

Then it classifies the orbit:

- $E<0$: elliptical orbit
- $E=0$: parabolic trajectory
- $E>0$: hyperbolic trajectory

---

## HTML Requirements

The HTML visualization should include:

- change of initial velocity
- graph of energy over time
- trajectory classification

---

## Conclusion

Newton's law of gravity describes motion in a central field:

$$F=-\frac{GMm}{r^2}$$

The total energy is:

$$E=\frac{1}{2}mv^2-\frac{GMm}{r}$$

The sign of the energy determines the orbit type.

If $E<0$, the body follows a bound elliptical orbit.

If $E=0$, the body follows a parabolic escape trajectory.

If $E>0$, the body follows a hyperbolic escape trajectory.

Thus, changing the initial velocity changes the total energy and determines whether the orbit is elliptical, parabolic, or hyperbolic.
