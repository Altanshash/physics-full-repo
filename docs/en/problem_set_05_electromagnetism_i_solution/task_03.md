# Problem 3 – Field at a Point from a System of Charges

## Given

Two point charges are given:

- charge $+q$ at point $(-a,0)$
- charge $+2q$ at point $(a,0)$

Find:

1. Electric field $\mathbf{E}(0,y)$, $\mathbf{E}(x,0)$, and $\mathbf{E}(x,y)$
2. Conditions for $E_x=0$, $E_y=0$, and $\mathbf{E}=0$
3. Field for $a=0.2 \ \text{m}$, $y=0.3 \ \text{m}$, $q=2 \ \mu\text{C}$
4. Limit when $y \gg a$
5. Does zero field exist on the $y$-axis?

---

## Solution

Electric field of a point charge:

$$
\mathbf{E}=kQ\frac{\mathbf{r}}{|\mathbf{r}|^3}
$$

---

## 1. Electric field at point $(0,y)$

For charge $+q$ at $(-a,0)$:

$$
\mathbf{r}_1=(a,y)
$$

For charge $+2q$ at $(a,0)$:

$$
\mathbf{r}_2=(-a,y)
$$

Total electric field:

$$
\mathbf{E}(0,y)
=
kq\frac{(a,y)}{(a^2+y^2)^{3/2}}
+
2kq\frac{(-a,y)}{(a^2+y^2)^{3/2}}
$$

$$
\mathbf{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}
\left((a,y)+2(-a,y)\right)
$$

$$
\mathbf{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

---

## 2. Electric field at point $(x,0)$

For charge $+q$:

$$
\mathbf{r}_1=(x+a,0)
$$

For charge $+2q$:

$$
\mathbf{r}_2=(x-a,0)
$$

So:

$$
\mathbf{E}(x,0)
=
kq\frac{x+a}{|x+a|^3}\mathbf{i}
+
2kq\frac{x-a}{|x-a|^3}\mathbf{i}
$$

---

## 3. Electric field at point $(x,y)$

For charge $+q$:

$$
\mathbf{r}_1=(x+a,y)
$$

For charge $+2q$:

$$
\mathbf{r}_2=(x-a,y)
$$

Therefore:

$$
\mathbf{E}(x,y)
=
kq\frac{(x+a,y)}{\left((x+a)^2+y^2\right)^{3/2}}
+
2kq\frac{(x-a,y)}{\left((x-a)^2+y^2\right)^{3/2}}
$$

Components:

$$
E_x
=
kq\frac{x+a}{\left((x+a)^2+y^2\right)^{3/2}}
+
2kq\frac{x-a}{\left((x-a)^2+y^2\right)^{3/2}}
$$

$$
E_y
=
kq\frac{y}{\left((x+a)^2+y^2\right)^{3/2}}
+
2kq\frac{y}{\left((x-a)^2+y^2\right)^{3/2}}
$$

---

## 4. Conditions for zero components

For $E_x=0$:

$$
\frac{x+a}{\left((x+a)^2+y^2\right)^{3/2}}
+
2\frac{x-a}{\left((x-a)^2+y^2\right)^{3/2}}
=
0
$$

For $E_y=0$:

$$
y
\left[
\frac{1}{\left((x+a)^2+y^2\right)^{3/2}}
+
\frac{2}{\left((x-a)^2+y^2\right)^{3/2}}
\right]
=
0
$$

Since the expression in brackets is always positive:

$$
E_y=0 \Rightarrow y=0
$$

So the zero electric field can only be on the $x$-axis.

---

## 5. Zero field point

On the $x$-axis:

$$
y=0
$$

Between the charges:

$$
-a<x<a
$$

Set the field magnitudes equal:

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
(a-x)^2=2(x+a)^2
$$

$$
a-x=\sqrt{2}(x+a)
$$

$$
x=a\frac{1-\sqrt{2}}{1+\sqrt{2}}
$$

This point is closer to the smaller charge $+q$.

---

## 6. Numerical calculation

Given:

$$
a=0.2 \ \text{m}
$$

$$
y=0.3 \ \text{m}
$$

$$
q=2 \ \mu\text{C}=2\times10^{-6} \ \text{C}
$$

Use:

$$
\mathbf{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

Calculate:

$$
a^2+y^2=(0.2)^2+(0.3)^2=0.13
$$

$$
(a^2+y^2)^{3/2}=0.13^{3/2}\approx0.0469
$$

$$
kq=(9\times10^9)(2\times10^{-6})=18000
$$

For the $x$-component:

$$
E_x=\frac{18000(-0.2)}{0.0469}
$$

$$
E_x\approx -7.67\times10^4 \ \text{N/C}
$$

For the $y$-component:

$$
E_y=\frac{18000(3)(0.3)}{0.0469}
$$

$$
E_y\approx 3.45\times10^5 \ \text{N/C}
$$

Therefore:

$$
\mathbf{E}(0,0.3)
\approx
(-7.67\times10^4,\ 3.45\times10^5) \ \text{N/C}
$$

---

## 7. Limit when $y \gg a$

When $y \gg a$:

$$
a^2+y^2 \approx y^2
$$

$$
(a^2+y^2)^{3/2}\approx y^3
$$

Then:

$$
\mathbf{E}(0,y)
\approx
\frac{kq}{y^3}(-a,3y)
$$

Since $a$ is very small compared with $y$:

$$
\mathbf{E}(0,y)
\approx
\left(0,\frac{3kq}{y^2}\right)
$$

This is like the field of total charge $3q$.

---

## 8. Zero field on the $y$-axis

On the $y$-axis:

$$
\mathbf{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

For zero field, both components must be zero.

But:

$$
E_x=
\frac{-akq}{(a^2+y^2)^{3/2}}
$$

Since $a\neq0$:

$$
E_x\neq0
$$

Therefore:

$$
\text{No zero field point exists on the } y\text{-axis.}
$$

---

## Final Answer

$$
\mathbf{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

$$
\mathbf{E}(x,0)
=
kq\frac{x+a}{|x+a|^3}\mathbf{i}
+
2kq\frac{x-a}{|x-a|^3}\mathbf{i}
$$

$$
\mathbf{E}(x,y)
=
kq\frac{(x+a,y)}{\left((x+a)^2+y^2\right)^{3/2}}
+
2kq\frac{(x-a,y)}{\left((x-a)^2+y^2\right)^{3/2}}
$$

$$
\mathbf{E}(0,0.3)
\approx
(-7.67\times10^4,\ 3.45\times10^5) \ \text{N/C}
$$

$$
x=a\frac{1-\sqrt{2}}{1+\sqrt{2}}
$$

Zero field does not exist on the $y$-axis.

---

## Conclusion

The total electric field is found by adding the electric fields from both charges.  
On the $y$-axis, the horizontal components do not cancel because the charges are different.  
Therefore, there is no zero field point on the $y$-axis.
