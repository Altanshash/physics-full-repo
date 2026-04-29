# Problem 3 – Field at a Point from a System of Charges

## Given

Two point charges are given:

$$
+q \text{ at } (-a,0)
$$

$$
+2q \text{ at } (a,0)
$$

Find:

1. Electric field \( \vec E(0,y) \), \( \vec E(x,0) \), and \( \vec E(x,y) \)
2. Conditions for \(E_x=0\), \(E_y=0\), and \(\vec E=0\)
3. Field for \(a=0.2 \ m\), \(y=0.3 \ m\), \(q=2 \ \mu C\)
4. Limit when \(y \gg a\)
5. Whether zero field exists on the \(y\)-axis

Coulomb constant:

$$
k = 9 \times 10^9 \ \frac{N \cdot m^2}{C^2}
$$

---

## Solution

For a point charge:

$$
\vec E = kq \frac{\vec r}{r^3}
$$

---

## 1. Field at \( (0,y) \)

From charge \(+q\):

$$
\vec r_1 = (a,y)
$$

From charge \(+2q\):

$$
\vec r_2 = (-a,y)
$$

So,

$$
\vec E(0,y)
=
kq \frac{(a,y)}{(a^2+y^2)^{3/2}}
+
k(2q)\frac{(-a,y)}{(a^2+y^2)^{3/2}}
$$

$$
\vec E(0,y)
=
\frac{kq}{(a^2+y^2)^{3/2}}
\left[(a,y)+2(-a,y)\right]
$$

$$
\boxed{
\vec E(0,y)=
\frac{kq}{(a^2+y^2)^{3/2}}
(-a,3y)
}
$$

---

## 2. Field at \( (x,0) \)

For charge \(+q\) at \((-a,0)\):

$$
\vec r_1 = (x+a,0)
$$

For charge \(+2q\) at \((a,0)\):

$$
\vec r_2 = (x-a,0)
$$

Therefore,

$$
\boxed{
\vec E(x,0)=
kq\frac{x+a}{|x+a|^3}\hat i
+
2kq\frac{x-a}{|x-a|^3}\hat i
}
$$

There is no \(y\)-component on the \(x\)-axis:

$$
\boxed{E_y=0}
$$

---

## 3. General field at \( (x,y) \)

From \(+q\):

$$
\vec r_1=(x+a,y)
$$

From \(+2q\):

$$
\vec r_2=(x-a,y)
$$

Thus,

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
\boxed{
E_x=
kq\frac{x+a}{\left[(x+a)^2+y^2\right]^{3/2}}
+
2kq\frac{x-a}{\left[(x-a)^2+y^2\right]^{3/2}}
}
$$

$$
\boxed{
E_y=
kq\frac{y}{\left[(x+a)^2+y^2\right]^{3/2}}
+
2kq\frac{y}{\left[(x-a)^2+y^2\right]^{3/2}}
}
$$

---

## 4. Conditions for zero components

For \(E_x=0\):

$$
kq\frac{x+a}{\left[(x+a)^2+y^2\right]^{3/2}}
+
2kq\frac{x-a}{\left[(x-a)^2+y^2\right]^{3/2}}
=0
$$

For \(E_y=0\):

$$
y\left[
\frac{1}{\left[(x+a)^2+y^2\right]^{3/2}}
+
\frac{2}{\left[(x-a)^2+y^2\right]^{3/2}}
\right]=0
$$

Since the bracket is positive:

$$
\boxed{E_y=0 \Rightarrow y=0}
$$

So zero field can only be on the \(x\)-axis.

---

## 5. Zero field point

On the \(x\)-axis, between charges:

$$
-a < x < a
$$

The fields are opposite.

Set:

$$
\frac{kq}{(x+a)^2}
=
\frac{2kq}{(a-x)^2}
$$

$$
(a-x)^2 = 2(x+a)^2
$$

Take square root:

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

This point is between the charges and closer to the smaller charge \(+q\).

---

## 6. Numerical calculation for \(a=0.2 \ m\), \(y=0.3 \ m\), \(q=2 \ \mu C\)

Use:

$$
\vec E(0,y)=
\frac{kq}{(a^2+y^2)^{3/2}}
(-a,3y)
$$

Substitute:

$$
a=0.2 \ m, \quad y=0.3 \ m
$$

$$
q=2\times10^{-6} \ C
$$

$$
a^2+y^2 = 0.2^2+0.3^2=0.13
$$

$$
(a^2+y^2)^{3/2}=0.13^{3/2}=0.0469
$$

$$
kq=(9\times10^9)(2\times10^{-6})=18000
$$

$$
E_x=\frac{18000(-0.2)}{0.0469}
$$

$$
E_x \approx -7.67\times10^4 \ \frac{N}{C}
$$

$$
E_y=\frac{18000(3)(0.3)}{0.0469}
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

## 7. Limit when \(y \gg a\)

If \(y \gg a\), then:

$$
a^2+y^2 \approx y^2
$$

So,

$$
(a^2+y^2)^{3/2} \approx y^3
$$

Then:

$$
\vec E(0,y)
\approx
\frac{kq}{y^3}(-a,3y)
$$

Since \(a \ll y\), the \(x\)-component is very small.

$$
\boxed{
\vec E(0,y)\approx
\left(0,\frac{3kq}{y^2}\right)
}
$$

This is like the field of total charge:

$$
q+2q=3q
$$

---

## 8. Does a zero field point exist on the \(y\)-axis?

On the \(y\)-axis:

$$
\vec E(0,y)=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
$$

For zero field:

$$
-a=0
$$

and

$$
3y=0
$$

But \(a \neq 0\). Therefore, both components cannot be zero.

$$
\boxed{\text{No zero field point exists on the } y\text{-axis.}}
$$

---

## Final Answer

$$
\boxed{
\vec E(0,y)=
\frac{kq}{(a^2+y^2)^{3/2}}(-a,3y)
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
