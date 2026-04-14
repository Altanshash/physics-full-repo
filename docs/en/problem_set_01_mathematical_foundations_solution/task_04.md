# Problem 4 – Geometry of parametric curves

## Given

Investigate the following curves:

### A)

$$
x(t) = R\cos t, \qquad y(t) = R\sin t
$$

### B)

$$
x(t) = a\cos t, \qquad y(t) = b\sin t
$$

### C)

$$
x(t) = t, \qquad y(t) = t^2
$$

### D)

$$
x(t) = \cosh t, \qquad y(t) = \sinh t
$$

For each curve we need to:

1. eliminate the parameter if possible,
2. determine the type of curve,
3. determine the velocity $\vec v(t)$ and acceleration $\vec a(t)$,
4. check whether $|\vec v|$ or $|\vec a|$ is constant.

---

# A) $x(t) = R\cos t$, $y(t) = R\sin t$

## 1. Eliminate the parameter

We have

$$
x = R\cos t, \qquad y = R\sin t
$$

Divide by $R$:

$$
\frac{x}{R} = \cos t, \qquad \frac{y}{R} = \sin t
$$

Square both equations and add them:

$$
\left(\frac{x}{R}\right)^2 + \left(\frac{y}{R}\right)^2 = \cos^2 t + \sin^2 t
$$

Since

$$
\cos^2 t + \sin^2 t = 1
$$

we get

$$
\frac{x^2}{R^2} + \frac{y^2}{R^2} = 1
$$

Thus,

$$
x^2 + y^2 = R^2
$$

## 2. Type of curve

This is a circle of radius $R$ centered at the origin.

## 3. Velocity and acceleration

The position vector is

$$
\vec r(t) = (R\cos t, R\sin t)
$$

Differentiate to get the velocity:

$$
\vec v(t) = (-R\sin t, R\cos t)
$$

Differentiate again to get the acceleration:

$$
\vec a(t) = (-R\cos t, -R\sin t)
$$

## 4. Magnitudes

Velocity magnitude:

$$
|\vec v| = \sqrt{(-R\sin t)^2 + (R\cos t)^2}
$$

$$
|\vec v| = \sqrt{R^2\sin^2 t + R^2\cos^2 t}
$$

$$
|\vec v| = \sqrt{R^2(\sin^2 t + \cos^2 t)} = \sqrt{R^2} = R
$$

So the speed is constant.

Acceleration magnitude:

$$
|\vec a| = \sqrt{(-R\cos t)^2 + (-R\sin t)^2}
$$

$$
|\vec a| = \sqrt{R^2\cos^2 t + R^2\sin^2 t}
$$

$$
|\vec a| = \sqrt{R^2(\cos^2 t + \sin^2 t)} = R
$$

So the acceleration magnitude is also constant.

### Final result for A

$$
x^2 + y^2 = R^2
$$

Circle of radius $R$.

$$
\vec v(t) = (-R\sin t, R\cos t)
$$

$$
\vec a(t) = (-R\cos t, -R\sin t)
$$

$$
|\vec v| = R \quad \text{constant}
$$

$$
|\vec a| = R \quad \text{constant}
$$

---

# B) $x(t) = a\cos t$, $y(t) = b\sin t$

## 1. Eliminate the parameter

We have

$$
x = a\cos t, \qquad y = b\sin t
$$

Divide by the constants:

$$
\frac{x}{a} = \cos t, \qquad \frac{y}{b} = \sin t
$$

Square and add:

$$
\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = \cos^2 t + \sin^2 t
$$

So,

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1
$$

## 2. Type of curve

This is an ellipse centered at the origin with semiaxes $a$ and $b$.

## 3. Velocity and acceleration

The position vector is

$$
\vec r(t) = (a\cos t, b\sin t)
$$

Differentiate:

$$
\vec v(t) = (-a\sin t, b\cos t)
$$

Differentiate again:

$$
\vec a(t) = (-a\cos t, -b\sin t)
$$

## 4. Magnitudes

Velocity magnitude:

$$
|\vec v| = \sqrt{(-a\sin t)^2 + (b\cos t)^2}
$$

$$
|\vec v| = \sqrt{a^2\sin^2 t + b^2\cos^2 t}
$$

This is not constant in general.

It is constant only if $a = b$, which reduces the ellipse to a circle.

Acceleration magnitude:

$$
|\vec a| = \sqrt{(-a\cos t)^2 + (-b\sin t)^2}
$$

$$
|\vec a| = \sqrt{a^2\cos^2 t + b^2\sin^2 t}
$$

This is also not constant in general.

It is constant only if $a = b$.

### Final result for B

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1
$$

Ellipse.

$$
\vec v(t) = (-a\sin t, b\cos t)
$$

$$
\vec a(t) = (-a\cos t, -b\sin t)
$$

$$
|\vec v| = \sqrt{a^2\sin^2 t + b^2\cos^2 t}
$$

$$
|\vec a| = \sqrt{a^2\cos^2 t + b^2\sin^2 t}
$$

In general, neither $|\vec v|$ nor $|\vec a|$ is constant.

---

# C) $x(t) = t$, $y(t) = t^2$

## 1. Eliminate the parameter

Since

$$
x = t
$$

we directly have

$$
t = x
$$

Substitute into $y = t^2$:

$$
y = x^2
$$

## 2. Type of curve

This is a parabola opening upward.

## 3. Velocity and acceleration

The position vector is

$$
\vec r(t) = (t, t^2)
$$

Differentiate:

$$
\vec v(t) = (1, 2t)
$$

Differentiate again:

$$
\vec a(t) = (0, 2)
$$

## 4. Magnitudes

Velocity magnitude:

$$
|\vec v| = \sqrt{1^2 + (2t)^2}
$$

$$
|\vec v| = \sqrt{1 + 4t^2}
$$

This is not constant.

Acceleration magnitude:

$$
|\vec a| = \sqrt{0^2 + 2^2} = 2
$$

This is constant.

### Final result for C

$$
y = x^2
$$

Parabola.

$$
\vec v(t) = (1, 2t)
$$

$$
\vec a(t) = (0, 2)
$$

$$
|\vec v| = \sqrt{1 + 4t^2}
$$

$$
|\vec a| = 2 \quad \text{constant}
$$

---

# D) $x(t) = \cosh t$, $y(t) = \sinh t$

## 1. Eliminate the parameter

We use the identity

$$
\cosh^2 t - \sinh^2 t = 1
$$

Since

$$
x = \cosh t, \qquad y = \sinh t
$$

we get

$$
x^2 - y^2 = 1
$$

## 2. Type of curve

This is a hyperbola.

More precisely, it is the right branch of the hyperbola $x^2 - y^2 = 1$, because $\cosh t \ge 1$ for all $t$.

## 3. Velocity and acceleration

The position vector is

$$
\vec r(t) = (\cosh t, \sinh t)
$$

Differentiate:

$$
\vec v(t) = (\sinh t, \cosh t)
$$

Differentiate again:

$$
\vec a(t) = (\cosh t, \sinh t)
$$

## 4. Magnitudes

Velocity magnitude:

$$
|\vec v| = \sqrt{(\sinh t)^2 + (\cosh t)^2}
$$

$$
|\vec v| = \sqrt{\sinh^2 t + \cosh^2 t}
$$

This depends on $t$, so it is not constant.

Acceleration magnitude:

$$
|\vec a| = \sqrt{(\cosh t)^2 + (\sinh t)^2}
$$

$$
|\vec a| = \sqrt{\cosh^2 t + \sinh^2 t}
$$

This also depends on $t$, so it is not constant.

### Final result for D

$$
x^2 - y^2 = 1
$$

Hyperbola, right branch.

$$
\vec v(t) = (\sinh t, \cosh t)
$$

$$
\vec a(t) = (\cosh t, \sinh t)
$$

$$
|\vec v| = \sqrt{\sinh^2 t + \cosh^2 t}
$$

$$
|\vec a| = \sqrt{\cosh^2 t + \sinh^2 t}
$$

Neither magnitude is constant.

---

# Final summary

## A)

$$
x^2 + y^2 = R^2
$$

Circle.

$$
\vec v(t) = (-R\sin t, R\cos t), \qquad \vec a(t) = (-R\cos t, -R\sin t)
$$

$$
|\vec v| = R, \qquad |\vec a| = R
$$

Both are constant.

## B)

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1
$$

Ellipse.

$$
\vec v(t) = (-a\sin t, b\cos t), \qquad \vec a(t) = (-a\cos t, -b\sin t)
$$

$$
|\vec v| = \sqrt{a^2\sin^2 t + b^2\cos^2 t}
$$

$$
|\vec a| = \sqrt{a^2\cos^2 t + b^2\sin^2 t}
$$

In general, neither is constant.

## C)

$$
y = x^2
$$

Parabola.

$$
\vec v(t) = (1, 2t), \qquad \vec a(t) = (0, 2)
$$

$$
|\vec v| = \sqrt{1 + 4t^2}
$$

$$
|\vec a| = 2
$$

Only the acceleration magnitude is constant.

## D)

$$
x^2 - y^2 = 1
$$

Hyperbola, right branch.

$$
\vec v(t) = (\sinh t, \cosh t), \qquad \vec a(t) = (\cosh t, \sinh t)
$$

$$
|\vec v| = \sqrt{\sinh^2 t + \cosh^2 t}
$$

$$
|\vec a| = \sqrt{\cosh^2 t + \sinh^2 t}
$$

Neither is constant.
