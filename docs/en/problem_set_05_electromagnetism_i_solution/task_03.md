# Problem 3 – Field at a Point from a System of Charges

## Given

Two point charges:

- charge $+q$ at $(-a,0)$
- charge $+2q$ at $(a,0)$

Find:

1. Electric field $\mathbf{E}(0,y)$, $\mathbf{E}(x,0)$, and $\mathbf{E}(x,y)$
2. Conditions for $E_x=0$, $E_y=0$, and $\mathbf{E}=0$
3. Field for $a=0.2 \text{ m}$, $y=0.3 \text{ m}$, $q=2 \mu C$
4. Limit when $y \gg a$
5. Does zero field exist on the $y$-axis?

---

## Solution

Electric field of a point charge:

```math
\mathbf{E}=kQ\frac{\mathbf{r}}{|\mathbf{r}|^3}
```

---

## 1. Field at point `(0,y)`

For charge $+q$:

```math
\mathbf{r}_1=(a,y)
```

For charge $+2q$:

```math
\mathbf{r}_2=(-a,y)
```

Total field:

```math
\mathbf{E}(0,y)
=
kq\frac{(a,y)}{(a^2+y^2)^{3/2}}
+
2kq\frac{(-a,y)}{(a^2+y^2)^{3/2}}
```

```math
\mathbf{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
```

---

## 2. Field at point `(x,0)`

```math
\mathbf{E}(x,0)
=
kq\frac{x+a}{|x+a|^3}\mathbf{i}
+
2kq\frac{x-a}{|x-a|^3}\mathbf{i}
```

---

## 3. Field at point `(x,y)`

```math
\mathbf{E}(x,y)
=
kq\frac{(x+a,y)}{\left((x+a)^2+y^2\right)^{3/2}}
+
2kq\frac{(x-a,y)}{\left((x-a)^2+y^2\right)^{3/2}}
```

Components:

```math
E_x
=
kq\frac{x+a}{\left((x+a)^2+y^2\right)^{3/2}}
+
2kq\frac{x-a}{\left((x-a)^2+y^2\right)^{3/2}}
```

```math
E_y
=
kq\frac{y}{\left((x+a)^2+y^2\right)^{3/2}}
+
2kq\frac{y}{\left((x-a)^2+y^2\right)^{3/2}}
```

---

## 4. Conditions

For $E_x=0$:

```math
\frac{x+a}{\left((x+a)^2+y^2\right)^{3/2}}
+
2\frac{x-a}{\left((x-a)^2+y^2\right)^{3/2}}
=
0
```

For $E_y=0$:

```math
y=0
```

So zero field can only be on the $x$-axis.

---

## 5. Zero field point

On the $x$-axis:

```math
y=0
```

Between the charges:

```math
-a<x<a
```

Set magnitudes equal:

```math
\frac{kq}{(x+a)^2}
=
\frac{2kq}{(a-x)^2}
```

```math
x
=
a\frac{1-\sqrt{2}}{1+\sqrt{2}}
```

---

## 6. Numerical calculation

Given:

```math
a=0.2 \text{ m}
```

```math
y=0.3 \text{ m}
```

```math
q=2\times10^{-6} \text{ C}
```

Use:

```math
\mathbf{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
```

Calculate:

```math
a^2+y^2=(0.2)^2+(0.3)^2=0.13
```

```math
(a^2+y^2)^{3/2}=0.13^{3/2}\approx0.0469
```

```math
kq=(9\times10^9)(2\times10^{-6})=18000
```

```math
E_x=\frac{18000(-0.2)}{0.0469}
\approx
-7.67\times10^4 \text{ N/C}
```

```math
E_y=\frac{18000(3)(0.3)}{0.0469}
\approx
3.45\times10^5 \text{ N/C}
```

Therefore:

```math
\mathbf{E}(0,0.3)
\approx
(-7.67\times10^4,\ 3.45\times10^5)\text{ N/C}
```

---

## 7. Limit when `y >> a`

When $y \gg a$:

```math
a^2+y^2\approx y^2
```

```math
(a^2+y^2)^{3/2}\approx y^3
```

So:

```math
\mathbf{E}(0,y)
\approx
\frac{kq}{y^3}(-a,3y)
```

Since $a$ is very small:

```math
\mathbf{E}(0,y)
\approx
\left(0,\frac{3kq}{y^2}\right)
```

---

## 8. Zero field on the y-axis

On the $y$-axis:

```math
\mathbf{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
```

But:

```math
E_x=
\frac{-akq}{(a^2+y^2)^{3/2}}
```

Since $a\neq0$:

```math
E_x\neq0
```

Therefore, zero field does not exist on the $y$-axis.

---

## Final Answer

```math
\mathbf{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
```

```math
\mathbf{E}(0,0.3)
\approx
(-7.67\times10^4,\ 3.45\times10^5)\text{ N/C}
```

```math
x
=
a\frac{1-\sqrt{2}}{1+\sqrt{2}}
```

Zero field does not exist on the $y$-axis.

---

## Conclusion

The total electric field is the vector sum of the fields from both charges.  
On the $y$-axis, the horizontal components do not cancel because the charges are different.  
Therefore, there is no zero field point on the $y$-axis.
