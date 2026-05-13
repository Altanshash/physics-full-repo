# Problem Set 9 – Model Cosmology: From Epicycles to Gravity

# Problem 1 – Ptolemy’s Model

## Given

The motion of a planet is represented as the sum of two circular motions:

1. Motion along the deferent (main circle)
2. Motion along the epicycle

The parametric equations are:

$$
x(t)=R\cos(\omega t)+r\cos(\Omega t)
$$

$$
y(t)=R\sin(\omega t)+r\sin(\Omega t)
$$

Where:

- \(R\) — radius of the deferent
- \(r\) — radius of the epicycle
- \(\omega\) — angular velocity of the deferent
- \(\Omega\) — angular velocity of the epicycle
- \(t\) — time

---

# Solution

## 1. Parametric Equations of the Trajectory

The position vector of the planet is the sum of the deferent motion and epicycle motion:

$$
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
$$

Therefore:

$$
x(t)=R\cos(\omega t)+r\cos(\Omega t)
$$

$$
y(t)=R\sin(\omega t)+r\sin(\Omega t)
$$

These equations describe the complete trajectory of the planet.

---

## 2. Angular Projection

The ecliptic longitude of the planet is:

$$
\varphi(t)=\operatorname{atan2}(y(t),x(t))
$$

Substituting the parametric equations:

$$
\varphi(t)=
\operatorname{atan2}
\left(
R\sin(\omega t)+r\sin(\Omega t),
R\cos(\omega t)+r\cos(\Omega t)
\right)
$$

---

## 3. Condition for Retrograde Motion

Retrograde motion occurs when the angular velocity changes direction:

$$
\frac{d\varphi}{dt}<0
$$

For a parametric curve:

$$
\frac{d\varphi}{dt}
=
\frac{x\dot{y}-y\dot{x}}{x^2+y^2}
$$

First, compute the derivatives:

$$
\dot{x}(t)
=
-R\omega\sin(\omega t)-r\Omega\sin(\Omega t)
$$

$$
\dot{y}(t)
=
R\omega\cos(\omega t)+r\Omega\cos(\Omega t)
$$

Retrograde motion occurs when:

$$
x\dot{y}-y\dot{x}<0
$$

After simplification:

$$
R^2\omega+r^2\Omega
+
Rr(\omega+\Omega)\cos((\omega-\Omega)t)
<0
$$

Thus, the condition for retrograde motion is:

$$
R^2\omega+r^2\Omega
+
Rr(\omega+\Omega)\cos((\omega-\Omega)t)
<0
$$

---

## 4. Moments of Direction Change

The direction changes when:

$$
\frac{d\varphi}{dt}=0
$$

Since \(x^2+y^2>0\), we solve:

$$
x\dot{y}-y\dot{x}=0
$$

Therefore:

$$
R^2\omega+r^2\Omega
+
Rr(\omega+\Omega)\cos((\omega-\Omega)t)
=0
$$

Solving for time:

$$
\cos((\omega-\Omega)t)
=
-\frac{R^2\omega+r^2\Omega}
{Rr(\omega+\Omega)}
$$

Hence:

$$
t_n=
\frac{
\pm
\arccos
\left(
-\frac{R^2\omega+r^2\Omega}
{Rr(\omega+\Omega)}
\right)
+2\pi n
}
{\omega-\Omega}
$$

Where:

$$
n\in\mathbb{Z}
$$

Solutions exist only if:

$$
\left|
\frac{R^2\omega+r^2\Omega}
{Rr(\omega+\Omega)}
\right|
\leq1
$$

---

# HTML Requirements

The interactive visualization must include:

- Sliders for:
  - \(R\)
  - \(r\)
  - \(\omega\)
  - \(\Omega\)

- Planet trajectory trace

- Graph of ecliptic longitude:

$$
\varphi(t)=\operatorname{atan2}(y(t),x(t))
$$

---

# Conclusion

Ptolemy’s model explains planetary motion using two circular motions: the deferent and the epicycle. Combining these motions produces complex trajectories that can reproduce apparent retrograde motion.

Retrograde motion occurs when:

$$
\frac{d\varphi}{dt}<0
$$

The moments when the apparent direction changes are obtained from:

$$
\frac{d\varphi}{dt}=0
$$

The behavior depends on the radii \(R\), \(r\) and angular velocities \(\omega\), \(\Omega\).
