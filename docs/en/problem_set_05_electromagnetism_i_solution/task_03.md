# Problem 3 – Field at a Point from a System of Charges

## Given

Two point charges:

- $+q$ is located at $(-a,0)$
- $+2q$ is located at $(a,0)$

Find:

1. Electric field $E(0,y)$, $E(x,0)$, and $E(x,y)$
2. Conditions for $E_x=0$, $E_y=0$, and $E=0$
3. Field for $a=0.2$ m, $y=0.3$ m, $q=2 \mu C$
4. Limit when $y \gg a$
5. Does zero field exist on the y-axis?

---

## Solution

Electric field of a point charge:

$$
E = kq \frac{r}{r^3}
$$

---

## 1. Field at point $(0,y)$

Distance from $+q$:

$$
r_1 = (a,y)
$$

Distance from $+2q$:

$$
r_2 = (-a,y)
$$

Total field:

$$
E(0,y)
=
kq \frac{(a,y)}{(a^2+y^2)^{3/2}}
+
2kq \frac{(-a,y)}{(a^2+y^2)^{3/2}}
$$

$$
E(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

---

## 2. Field at point $(x,0)$

$$
E(x,0)
=
kq \frac{x+a}{|x+a|^3}
+
2kq \frac{x-a}{|x-a|^3}
$$

---

## 3. Field at point $(x,y)$

$$
E(x,y)
=
kq \frac{(x+a,y)}{((x+a)^2+y^2)^{3/2}}
+
2kq \frac{(x-a,y)}{((x-a)^2+y^2)^{3/2}}
$$

Components:

$$
E_x
=
kq \frac{x+a}{((x+a)^2+y^2)^{3/2}}
+
2kq \frac{x-a}{((x-a)^2+y^2)^{3/2}}
$$

$$
E_y
=
kq \frac{y}{((x+a)^2+y^2)^{3/2}}
+
2kq \frac{y}{((x-a)^2+y^2)^{3/2}}
$$

---

## 4. Conditions

For $E_x=0$:

$$
\frac{x+a}{((x+a)^2+y^2)^{3/2}}
+
2\frac{x-a}{((x-a)^2+y^2)^{3/2}}
=
0
$$

For $E_y=0$:

$$
y
\left[
\frac{1}{((x+a)^2+y^2)^{3/2}}
+
\frac{2}{((x-a)^2+y^2)^{3/2}}
\right]
=
0
$$

Therefore:

$$
E_y=0
$$

when:

$$
y=0
$$

So the zero field point can only be on the x-axis.

---

## 5. Zero field point

On the x-axis:

$$
y=0
$$

Between the charges:

$$
-a < x < a
$$

Set fields equal:

$$
\frac{kq}{(x+a)^2}
=
\frac{2kq}{(a-x)^2}
$$

Cancel $kq$:

$$
\frac{1}{(x+a)^2}
=
\frac{2}{(a-x)^2}
$$

$$
(a-x)^2 = 2(x+a)^2
$$

$$
a-x = \sqrt{2}(x+a)
$$

$$
x = a\frac{1-\sqrt{2}}{1+\sqrt{2}}
$$

---

## 6. Numerical calculation

Given:

$$
a=0.2 \ m
$$

$$
y=0.3 \ m
$$

$$
q=2 \times 10^{-6} \ C
$$

Use:

$$
E(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

Calculate:

$$
a^2+y^2 = 0.2^2+0.3^2 = 0.13
$$

$$
(a^2+y^2)^{3/2} = 0.0469
$$

$$
kq = (9\times10^9)(2\times10^{-6}) = 18000
$$

For $E_x$:

$$
E_x = \frac{18000(-0.2)}{0.0469}
$$

$$
E_x = -7.67\times10^4 \ N/C
$$

For $E_y$:

$$
E_y = \frac{18000(0.9)}{0.0469}
$$

$$
E_y = 3.45\times10^5 \ N/C
$$

So:

$$
E(0,0.3)
=
(-7.67\times10^4,\ 3.45\times10^5) \ N/C
$$

---

## 7. Limit when $y \gg a$

When $y \gg a$:

$$
a^2+y^2 \approx y^2
$$

$$
(a^2+y^2)^{3/2} \approx y^3
$$

Then:

$$
E(0,y)
\approx
\frac{kq}{y^3}(-a,3y)
$$

Since $a$ is very small:

$$
E(0,y)
\approx
\left(0,\frac{3kq}{y^2}\right)
$$

---

## 8. Zero field on the y-axis

On the y-axis:

$$
E(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

For zero field, both components must be zero.

But:

$$
E_x =
\frac{-akq}{(a^2+y^2)^{3/2}}
$$

Since $a \neq 0$:

$$
E_x \neq 0
$$

Therefore, zero field does not exist on the y-axis.

---

## Final Answer

$$
E(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

$$
E(0,0.3)
=
(-7.67\times10^4,\ 3.45\times10^5) \ N/C
$$

$$
x = a\frac{1-\sqrt{2}}{1+\sqrt{2}}
$$

Zero field does not exist on the y-axis.

---

## Conclusion

The electric field is found by adding the fields from both charges.  
On the y-axis, the horizontal components do not cancel because the charges are different.  
So there is no zero field point on the y-axis.
