# Problem Set 9 – Model Cosmology: From Epicycles to Gravity

## Problem 1 – Ptolemy's Model

## Given

The motion of a planet is represented as the sum of two circular motions:

1. Motion along the deferent, or main circle.
2. Motion along the epicycle.

The parametric equations are:

\[
x(t)=R\cos(\omega t)+r\cos(\Omega t)
\]

\[
y(t)=R\sin(\omega t)+r\sin(\Omega t)
\]

where:

- \(R\) is the radius of the deferent,
- \(r\) is the radius of the epicycle,
- \(\omega\) is the angular velocity of the deferent,
- \(\Omega\) is the angular velocity of the epicycle,
- \(t\) is time.

---

## Solution

### 1. Parametric Equations of the Trajectory

The position of the planet is the sum of the deferent motion and epicycle motion:

\[
\vec{r}(t)=
\begin{pmatrix}
R\cos(\omega t) \\
R\sin(\omega t)
\end{pmatrix}
+
\begin{pmatrix}
r\cos(\Omega t) \\
r\sin(\Omega t)
\end{pmatrix}
\]

Therefore,

\[
x(t)=R\cos(\omega t)+r\cos(\Omega t)
\]

\[
y(t)=R\sin(\omega t)+r\sin(\Omega t)
\]

These equations describe the full trajectory of the planet.

---

### 2. Angular Projection

The ecliptic longitude is the angle of the planet measured from the origin:

\[
\varphi(t)=\tan^{-1}\left(\frac{y(t)}{x(t)}\right)
\]

More accurately, it should be written using the two-argument arctangent:

\[
\varphi(t)=\operatorname{atan2}(y(t),x(t))
\]

Substituting \(x(t)\) and \(y(t)\):

\[
\varphi(t)=
\operatorname{atan2}
\left(
R\sin(\omega t)+r\sin(\Omega t),
R\cos(\omega t)+r\cos(\Omega t)
\right)
\]

---

### 3. Condition for Retrograde Motion

Retrograde motion occurs when the apparent angular motion changes direction.

This means:

\[
\frac{d\varphi}{dt}<0
\]

For a parametric curve, the angular velocity is:

\[
\frac{d\varphi}{dt}
=
\frac{x\dot{y}-y\dot{x}}{x^2+y^2}
\]

First, find the derivatives:

\[
\dot{x}(t)
=
-R\omega\sin(\omega t)-r\Omega\sin(\Omega t)
\]

\[
\dot{y}(t)
=
R\omega\cos(\omega t)+r\Omega\cos(\Omega t)
\]

Thus, retrograde motion occurs when:

\[
x\dot{y}-y\dot{x}<0
\]

After simplification:

\[
R^2\omega+r^2\Omega+Rr(\omega+\Omega)\cos((\omega-\Omega)t)<0
\]

So the condition for retrograde motion is:

\[
R^2\omega+r^2\Omega+Rr(\omega+\Omega)\cos((\omega-\Omega)t)<0
\]

---

### 4. Moments of Change in Direction

The direction of angular motion changes when:

\[
\frac{d\varphi}{dt}=0
\]

Since \(x^2+y^2>0\), this happens when:

\[
x\dot{y}-y\dot{x}=0
\]

Therefore:

\[
R^2\omega+r^2\Omega+Rr(\omega+\Omega)\cos((\omega-\Omega)t)=0
\]

Solving for time:

\[
\cos((\omega-\Omega)t)
=
-\frac{R^2\omega+r^2\Omega}{Rr(\omega+\Omega)}
\]

The moments of change in direction are:

\[
t_n=
\frac{
\pm \arccos\left(
-\frac{R^2\omega+r^2\Omega}{Rr(\omega+\Omega)}
\right)+2\pi n
}
{\omega-\Omega}
\]

where \(n\in\mathbb{Z}\).

These moments exist only if:

\[
\left|
\frac{R^2\omega+r^2\Omega}{Rr(\omega+\Omega)}
\right|
\leq 1
\]

---

## HTML Requirements

The interactive model should include:

- Sliders for:
  - \(R\)
  - \(r\)
  - \(\omega\)
  - \(\Omega\)

- A trajectory trace of the planet.

- A graph of the ecliptic longitude:

\[
\varphi(t)=\operatorname{atan2}(y(t),x(t))
\]

---

## Conclusion

Ptolemy's model describes planetary motion as a combination of two circular motions: motion along the deferent and motion along the epicycle. The resulting trajectory can explain loops and apparent retrograde motion.

Retrograde motion occurs when the angular velocity of the planet becomes negative:

\[
\frac{d\varphi}{dt}<0
\]

The moments when the planet changes its apparent direction are found by setting:

\[
\frac{d\varphi}{dt}=0
\]

This shows that retrograde motion is not random, but depends on the radii \(R\), \(r\), and angular velocities \(\omega\), \(\Omega\).
