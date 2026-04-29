# Problem 3 – Field at a Point from a System of Charges

## Given

Two point charges are given:

- charge $+q$ at point $(-a,0)$
- charge $+2q$ at point $(a,0)$

Find:

1. Electric field $\vec E(0,y)$, $\vec E(x,0)$, and $\vec E(x,y)$
2. Conditions for $E_x = 0$, $E_y = 0$, and $\vec E = 0$
3. Field for $a = 0.2 \ m$, $y = 0.3 \ m$, $q = 2 \ \mu C$
4. Limit when $y \gg a$
5. Whether zero field exists on the $y$-axis

Coulomb constant:

$$
k = 9 \times 10^9 \ \frac{N \cdot m^2}{C^2}
$$

---

## Solution

The electric field of one point charge is:

$$
\vec E = kq \frac{\vec r}{r^3}
$$

---

## 1. Electric field at point $(0,y)$

For charge $+q$:

$$
\vec r_1 = (a,y)
$$

For charge $+2q$:

$$
\vec r_2 = (-a,y)
$$

So,

$$
\vec E(0,y)
=
kq \frac{(a,y)}{(a^2+y^2)^{3/2}}
+
2kq \frac{(-a,y)}{(a^2+y^2)^{3/2}}
$$

$$
\vec E(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}
\left[(a,y)+2(-a,y)\right]
$$

$$
\boxed{
\vec E(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
}
$$

---

## 2. Electric field at point $(x,0)$

For charge $+q$:

$$
\vec r_1 = (x+a,0)
$$

For charge $+2q$:

$$
\vec r_2 = (x-a,0)
$$

Therefore,

$$
\boxed{
\vec E(x,0)
=
kq \frac{x+a}{|x+a|^3}\hat i
+
2kq \frac{x-a}{|x-a|^3}\hat i
}
$$

---

## 3. General electric field at point $(x,y)$

For charge $+q$:

$$
\vec r_1 = (x+a,y)
$$

For charge $+2q$:

$$
\vec r_2 = (x-a,y)
$$

Therefore,

$$
\boxed{
\vec E(x,y)
=
kq\frac{(x+a,y)}{\left[(x+a)^2+y^2\right]^{3/2}}
+
2kq\frac{(x-a,y)}{\left[(x-a)^2+y^2\right]^{3/2}}
}
$$

Components:

$$
E_x
=
kq\frac{x+a}{\left[(x+a)^2+y^2\right]^{3/2}}
+
2kq\frac{x-a}{\left[(x-a)^2+y^2\right]^{3/2}}
$$

$$
E_y
=
kq\frac{y}{\left[(x+a)^2+y^2\right]^{3/2}}
+
2kq\frac{y}{\left[(x-a)^2+y^2\right]^{3/2}}
$$

---

## 4. Conditions for zero components

For $E_x = 0$:

$$
\frac{x+a}{\left[(x+a)^2+y^2\right]^{3/2}}
+
2\frac{x-a}{\left[(x-a)^2+y^2\right]^{3/2}}
=
0
$$

For $E_y = 0$:

$$
y
\left[
\frac{1}{\left[(x+a)^2+y^2\right]^{3/2}}
+
\frac{2}{\left[(x-a)^2+y^2\right]^{3/2}}
\right]
=
0
$$

Since the expression in brackets is always positive:

$$
\boxed{E_y = 0 \Rightarrow y = 0}
$$

So the zero field point can only be on the $x$-axis.

---

## 5. Zero field point

On the $x$-axis, the zero field point is between the charges:

$$
-a < x < a
$$

The fields are opposite there, so:

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

So,

$$
\boxed{
x = a\frac{1-\sqrt{2}}{1+\sqrt{2}}
}
$$

---

## 6. Numerical calculation

Given:

$$
a = 0.2 \ m
$$

$$
y = 0.3 \ m
$$

$$
q = 2 \ \mu C = 2 \times 10^{-6} \ C
$$

Use:

$$
\vec E(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

Calculate:

$$
a^2+y^2 = (0.2)^2+(0.3)^2 = 0.13
$$

$$
(a^2+y^2)^{3/2} = 0.13^{3/2} \approx 0.0469
$$

$$
kq = (9\times10^9)(2\times10^{-6}) = 18000
$$

For $E_x$:

$$
E_x = \frac{18000(-0.2)}{0.0469}
$$

$$
E_x \approx -7.67\times10^4 \ \frac{N}{C}
$$

For $E_y$:

$$
E_y = \frac{18000(3)(0.3)}{0.0469}
$$

$$
E_y \approx 3.45\times10^5 \ \frac{N}{C}
$$

Therefore,

$$
\boxed{
\vec E(0,0.3)
\approx
(-7.67\times10^4,\ 3.45\times10^5)
\ \frac{N}{C}
}
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
\vec E(0,y)
\approx
\frac{kq}{y^3}(-a,3y)
$$

Since $a$ is very small compared with $y$, the $x$-component becomes very small:

$$
\boxed{
\vec E(0,y)
\approx
\left(0,\frac{3kq}{y^2}\right)
}
$$

This is like the field of one total charge:

$$
q_{\text{total}} = q + 2q = 3q
$$

---

## 8. Zero field on the $y$-axis

On the $y$-axis:

$$
\vec E(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

For zero field:

$$
E_x = 0
$$

and

$$
E_y = 0
$$

But:

$$
E_x =
\frac{-akq}{(a^2+y^2)^{3/2}}
$$

Since $a \neq 0$, then:

$$
E_x \neq 0
$$

Therefore:

$$
\boxed{
\text{No zero field point exists on the } y\text{-axis.}
}
$$

---

## Final Answer

$$
\boxed{
\vec E(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
}
$$

$$
\boxed{
\vec E(x,0)
=
kq \frac{x+a}{|x+a|^3}\hat i
+
2kq \frac{x-a}{|x-a|^3}\hat i
}
$$

$$
\boxed{
\vec E(x,y)
=
kq\frac{(x+a,y)}{\left[(x+a)^2+y^2\right]^{3/2}}
+
2kq\frac{(x-a,y)}{\left[(x-a)^2+y^2\right]^{3/2}}
}
$$

$$
\boxed{
\vec E(0,0.3)
\approx
(-7.67\times10^4,\ 3.45\times10^5)
\ \frac{N}{C}
}
$$

$$
\boxed{
\text{Zero field does not exist on the } y\text{-axis.}
}
$$

---

## Conclusion

The electric field is found by adding the fields from both charges.  
On the $y$-axis, the vertical components add, but the horizontal components do not cancel because the charges are different.  
Therefore, there is no zero field point on the $y$-axis.
