# Problem Set 9 – Model Cosmology: From Epicycles to Gravity

# Problem 1 – Ptolemy’s Model

## Given

The motion of a planet is represented as the sum of two circular motions:

1. Motion along the deferent, which is the main circle.
2. Motion along the epicycle.

The parametric equations are:

$$
x(t)=R\cos(\omega t)+r\cos(\Omega t)
$$

$$
y(t)=R\sin(\omega t)+r\sin(\Omega t)
$$

Where:

- $R$ is the radius of the deferent.
- $r$ is the radius of the epicycle.
- $\omega$ is the angular velocity of the deferent.
- $\Omega$ is the angular velocity of the epicycle.
- $t$ is time.

---

# Solution

## 1. Parametric Equations of the Trajectory

The position of the planet is the sum of the deferent motion and the epicycle motion.

For the deferent:

$$
x_1(t)=R\cos(\omega t)
$$

$$
y_1(t)=R\sin(\omega t)
$$

For the epicycle:

$$
x_2(t)=r\cos(\Omega t)
$$

$$
y_2(t)=r\sin(\Omega t)
$$

Adding these two motions gives:

$$
x(t)=x_1(t)+x_2(t)
$$

$$
y(t)=y_1(t)+y_2(t)
$$

Therefore:

$$
x(t)=R\cos(\omega t)+r\cos(\Omega t)
$$

$$
y(t)=R\sin(\omega t)+r\sin(\Omega t)
$$

These equations describe the trajectory of the planet.

---

## 2. Ecliptic Longitude

The ecliptic longitude is the angle of the planet measured from the origin.

It is given by:

$$
\varphi(t)=\arctan\left(\frac{y(t)}{x(t)}\right)
$$

Substituting $x(t)$ and $y(t)$:

$$
\varphi(t)=
\arctan\left(
\frac{
R\sin(\omega t)+r\sin(\Omega t)
}{
R\cos(\omega t)+r\cos(\Omega t)
}
\right)
$$

This function describes the angular position of the planet as seen from the origin.

---

## 3. Condition for Retrograde Motion

Retrograde motion occurs when the apparent angular motion becomes negative.

Therefore, the condition is:

$$
\frac{d\varphi}{dt}<0
$$

For a parametric curve, the angular velocity is:

$$
\frac{d\varphi}{dt}
=
\frac{x(t)y'(t)-y(t)x'(t)}
{x^2(t)+y^2(t)}
$$

Now find the derivatives:

$$
x'(t)
=
-R\omega\sin(\omega t)-r\Omega\sin(\Omega t)
$$

$$
y'(t)
=
R\omega\cos(\omega t)+r\Omega\cos(\Omega t)
$$

Since the denominator $x^2(t)+y^2(t)$ is positive, retrograde motion occurs when:

$$
x(t)y'(t)-y(t)x'(t)<0
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

## 4. Moments of Change in Direction

The direction of motion changes when the angular velocity becomes zero:

$$
\frac{d\varphi}{dt}=0
$$

This gives:

$$
x(t)y'(t)-y(t)x'(t)=0
$$

So:

$$
R^2\omega+r^2\Omega
+
Rr(\omega+\Omega)\cos((\omega-\Omega)t)
=0
$$

Solving for the cosine term:

$$
\cos((\omega-\Omega)t)
=
-\frac{R^2\omega+r^2\Omega}
{Rr(\omega+\Omega)}
$$

Therefore, the moments of direction change are:

$$
t_n=
\frac{
\pm\arccos\left(
-\frac{R^2\omega+r^2\Omega}
{Rr(\omega+\Omega)}
\right)
+2\pi n
}
{\omega-\Omega}
$$

Where:

$$
n\in Z
$$

Such moments exist only if:

$$
\left|
\frac{R^2\omega+r^2\Omega}
{Rr(\omega+\Omega)}
\right|
\leq 1
$$

---

# HTML Requirements

The HTML model must include:

- Sliders for $R$, $r$, $\omega$, and $\Omega$
- A trajectory trace of the planet
- A graph of the ecliptic longitude $\varphi(t)$

The ecliptic longitude is:

$$
\varphi(t)=
\arctan\left(
\frac{
R\sin(\omega t)+r\sin(\Omega t)
}{
R\cos(\omega t)+r\cos(\Omega t)
}
\right)
$$

---

# Conclusion

Ptolemy’s model describes the motion of a planet as a combination of two circular motions: motion along the deferent and motion along the epicycle.

The trajectory is described by:

$$
x(t)=R\cos(\omega t)+r\cos(\Omega t)
$$

$$
y(t)=R\sin(\omega t)+r\sin(\Omega t)
$$

Retrograde motion occurs when the angular velocity is negative:

$$
\frac{d\varphi}{dt}<0
$$

The moments when the planet changes its apparent direction are found from:

$$
\frac{d\varphi}{dt}=0
$$

Thus, the appearance of retrograde motion depends on the values of $R$, $r$, $\omega$, and $\Omega$.
