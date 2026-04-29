# Problem 3 – Field at a Point from a System of Charges

## Given

Two point charges are given:

- $+q$ at $(-a,0)$
- $+2q$ at $(a,0)$

Find:

1. Electric field $\vec{E}(0,y)$, $\vec{E}(x,0)$, and $\vec{E}(x,y)$
2. Conditions for $E_x = 0$, $E_y = 0$, and $\vec{E}=0$
3. Field for $a=0.2 \ \text{m}$, $y=0.3 \ \text{m}$, $q=2 \ \mu\text{C}$
4. Limit when $y \gg a$
5. Does a zero field point exist on the $y$-axis?

---

## Solution

Electric field of a point charge:

$$
\vec{E}=kq\frac{\vec{r}}{r^3}
$$

---

## 1. Field at $(0,y)$

For charge $+q$ at $(-a,0)$:

$$
\vec{r}_1=(a,y)
$$

For charge $+2q$ at $(a,0)$:

$$
\vec{r}_2=(-a,y)
$$

Therefore:

$$
\vec{E}(0,y)
=
kq\frac{(a,y)}{(a^2+y^2)^{3/2}}
+
2kq\frac{(-a,y)}{(a^2+y^2)^{3/2}}
$$

$$
\boxed{
\vec{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
}
$$

---

## 2. Field at $(x,0)$

$$
\boxed{
\vec{E}(x,0)
=
kq\frac{x+a}{|x+a|^3}\hat{i}
+
2kq\frac{x-a}{|x-a|^3}\hat{i}
}
$$

---

## 3. Field at $(x,y)$

$$
\boxed{
\vec{E}(x,y)
=
kq\frac{(x+a,y)}{\left((x+a)^2+y^2\right)^{3/2}}
+
2kq\frac{(x-a,y)}{\left((x-a)^2+y^2\right)^{3/2}}
}
$$

So,

$$
E_x=
kq\frac{x+a}{\left((x+a)^2+y^2\right)^{3/2}}
+
2kq\frac{x-a}{\left((x-a)^2+y^2\right)^{3/2}}
$$

$$
E_y=
kq\frac{y}{\left((x+a)^2+y^2\right)^{3/2}}
+
2kq\frac{y}{\left((x-a)^2+y^2\right)^{3/2}}
$$

---

## 4. Conditions

For $E_x=0$:

$$
\frac{x+a}{\left((x+a)^2+y^2\right)^{3/2}}
+
2\frac{x-a}{\left((x-a)^2+y^2\right)^{3/2}}
=0
$$

For $E_y=0$:

$$
y
\left[
\frac{1}{\left((x+a)^2+y^2\right)^{3/2}}
+
\frac{2}{\left((x-a)^2+y^2\right)^{3/2}}
\right]
=0
$$

Since the bracket is positive:

$$
\boxed{E_y=0 \Rightarrow y=0}
$$

So $\vec{E}=0$ can only be on the $x$-axis.

---

## 5. Zero field point

On the $x$-axis:

$$
y=0
$$

The zero field point is between the charges:

$$
-a<x<a
$$

Set magnitudes equal:

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

$$
\boxed{
x=a\frac{1-\sqrt{2}}{1+\sqrt{2}}
}
$$

---

## 6. Numerical value

Given:

$$
a=0.2 \ \text{m}
$$

$$
y=0.3 \ \text{m}
$$

$$
q=2\times10^{-6} \ \text{C}
$$

Use:

$$
\vec{E}(0,y)
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

Then:

$$
E_x=\frac{18000(-0.2)}{0.0469}
\approx -7.67\times10^4 \ \text{N/C}
$$

$$
E_y=\frac{18000(0.9)}{0.0469}
\approx 3.45\times10^5 \ \text{N/C}
$$

Therefore:

$$
\boxed{
\vec{E}(0,0.3)
=
(-7.67\times10^4,\ 3.45\times10^5) \ \text{N/C}
}
$$

---

## 7. Limit when $y \gg a$

When $y \gg a$:

$$
a^2+y^2 \approx y^2
$$

So:

$$
(a^2+y^2)^{3/2} \approx y^3
$$

Then:

$$
\vec{E}(0,y)
\approx
\frac{kq}{y^3}(-a,3y)
$$

Since $a$ is very small:

$$
\boxed{
\vec{E}(0,y)
\approx
\left(0,\frac{3kq}{y^2}\right)
}
$$

---

## 8. Zero field on the $y$-axis

On the $y$-axis:

$$
\vec{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

For zero field, both components must be zero.

But:

$$
E_x=
\frac{-akq}{(a^2+y^2)^{3/2}}
$$

Since $a \neq 0$:

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
\vec{E}(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
}
$$

$$
\boxed{
\vec{E}(0,0.3)
=
(-7.67\times10^4,\ 3.45\times10^5) \ \text{N/C}
}
$$

$$
\boxed{
\text{No zero field point exists on the } y\text{-axis.}
}
$$

---

## Conclusion

The electric field is the sum of the fields from both charges.  
Because the charges are not equal, the horizontal components on the $y$-axis do not cancel.  
So there is no zero field point on the $y$-axis.
