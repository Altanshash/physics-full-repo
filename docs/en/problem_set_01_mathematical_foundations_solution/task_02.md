## Problem 1 – Vectors and linear transformations

### Given

We are given two vectors in $\mathbb{R}^3$:

$$
\vec{a} = (2,-1,3), \qquad \vec{b} = (1,4,-2)
$$

and the matrix

$$
A=
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}.
$$

We will compute the vector lengths, the normalized vector, the dot product, the angle, the cross product, the parallelogram area, the product $A\vec{a}$, the determinant of $A$, and the orientation of the transformation.

---

## 1. Lengths of the vectors

The length of a vector $(x,y,z)$ is

$$
|(x,y,z)|=\sqrt{x^2+y^2+z^2}.
$$

For $\vec{a}=(2,-1,3)$:

$$
|\vec{a}|=\sqrt{2^2+(-1)^2+3^2}
=\sqrt{4+1+9}
=\sqrt{14}.
$$

So,

$$
\boxed{|\vec{a}|=\sqrt{14}}.
$$

For $\vec{b}=(1,4,-2)$:

$$
|\vec{b}|=\sqrt{1^2+4^2+(-2)^2}
=\sqrt{1+16+4}
=\sqrt{21}.
$$

Thus,

$$
\boxed{|\vec{b}|=\sqrt{21}}.
$$

---

## 2. Normalized vector $\hat{a}$

The normalized vector is defined by

$$
\hat{a}=\frac{\vec{a}}{|\vec{a}|}.
$$

Since $|\vec{a}|=\sqrt{14}$, we get

$$
\hat{a}=\frac{(2,-1,3)}{\sqrt{14}}
=
\left(
\frac{2}{\sqrt{14}},
-\frac{1}{\sqrt{14}},
\frac{3}{\sqrt{14}}
\right).
$$

Hence,

$$
\boxed{
\hat{a}=
\left(
\frac{2}{\sqrt{14}},
-\frac{1}{\sqrt{14}},
\frac{3}{\sqrt{14}}
\right)
}.
$$

---

## 3. Dot product and the angle between the vectors

The dot product is

$$
\vec{a}\cdot\vec{b}
=2\cdot1+(-1)\cdot4+3\cdot(-2).
$$

Now calculate term by term:

$$
\vec{a}\cdot\vec{b}=2-4-6=-8.
$$

Therefore,

$$
\boxed{\vec{a}\cdot\vec{b}=-8}.
$$

The angle $\theta$ between the vectors satisfies

$$
\cos\theta=\frac{\vec{a}\cdot\vec{b}}{|\vec{a}||\vec{b}|}.
$$

Substituting the known values:

$$
\cos\theta=\frac{-8}{\sqrt{14}\sqrt{21}}
=\frac{-8}{\sqrt{294}}.
$$

So the angle is

$$
\theta=\arccos\left(\frac{-8}{\sqrt{294}}\right).
$$

Numerically,

$$
\theta \approx 117.9^\circ.
$$

Thus,

$$
\boxed{
\theta=\arccos\left(\frac{-8}{\sqrt{294}}\right)\approx117.9^\circ
}.
$$

---

## 4. Cross product and the area of the parallelogram

The cross product is

$$
\vec{a}\times\vec{b}
=
\begin{pmatrix}
a_2b_3-a_3b_2 \\
a_3b_1-a_1b_3 \\
a_1b_2-a_2b_1
\end{pmatrix}.
$$

For $\vec{a}=(2,-1,3)$ and $\vec{b}=(1,4,-2)$:

$$
\vec{a}\times\vec{b}
=
\begin{pmatrix}
(-1)(-2)-3\cdot4 \\
3\cdot1-2(-2) \\
2\cdot4-(-1)\cdot1
\end{pmatrix}
=
\begin{pmatrix}
2-12 \\
3+4 \\
8+1
\end{pmatrix}
=
\begin{pmatrix}
-10 \\
7 \\
9
\end{pmatrix}.
$$

So,

$$
\boxed{\vec{a}\times\vec{b}=(-10,7,9)}.
$$

The area of the parallelogram is the magnitude of the cross product:

$$
|\vec{a}\times\vec{b}|
=\sqrt{(-10)^2+7^2+9^2}
=\sqrt{100+49+81}
=\sqrt{230}.
$$

Therefore,

$$
\boxed{\text{Area}=\sqrt{230}\approx15.17}.
$$

---

## 5. Calculation of $A\vec{a}$

We multiply the matrix by the vector:

$$
A\vec{a}
=
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
2 \\
-1 \\
3
\end{pmatrix}.
$$

Now compute each row:

$$
\begin{aligned}
\text{Row 1: } & 2\cdot2+1\cdot(-1)+0\cdot3=4-1=3, \\
\text{Row 2: } & 0\cdot2+1\cdot(-1)-1\cdot3=-1-3=-4, \\
\text{Row 3: } & 1\cdot2+0\cdot(-1)+1\cdot3=2+3=5.
\end{aligned}
$$

Thus,

$$
A\vec{a}
=
\begin{pmatrix}
3 \\
-4 \\
5
\end{pmatrix}.
$$

Hence,

$$
\boxed{A\vec{a}=(3,-4,5)}.
$$

---

## 6. Determinant of the matrix

We compute the determinant by expanding along the first row:

$$
\det A=
\begin{vmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{vmatrix}.
$$

So,

$$
\det A
=
2
\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
-
1
\begin{vmatrix}
0 & -1 \\
1 & 1
\end{vmatrix}
+
0
\begin{vmatrix}
0 & 1 \\
1 & 0
\end{vmatrix}.
$$

Now evaluate the $2\times2$ determinants:

$$
\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
=1\cdot1-(-1)\cdot0=1,
$$

$$
\begin{vmatrix}
0 & -1 \\
1 & 1
\end{vmatrix}
=0\cdot1-(-1)\cdot1=1.
$$

Therefore,

$$
\det A = 2\cdot1 - 1\cdot1 + 0 = 1.
$$

So,

$$
\boxed{\det A=1}.
$$

---

## 7. Orientation of the transformation

A linear transformation preserves orientation if its determinant is positive.

Since

$$
\det A=1>0,
$$

the transformation preserves the orientation of space.

Thus,

$$
\boxed{\text{The transformation preserves orientation}.}
$$

---

## Final answers

$$
\boxed{|\vec{a}|=\sqrt{14}}, \qquad
\boxed{|\vec{b}|=\sqrt{21}}
$$

$$
\boxed{
\hat{a}=
\left(
\frac{2}{\sqrt{14}},
-\frac{1}{\sqrt{14}},
\frac{3}{\sqrt{14}}
\right)
}
$$

$$
\boxed{\vec{a}\cdot\vec{b}=-8}
$$

$$
\boxed{
\theta=\arccos\left(\frac{-8}{\sqrt{294}}\right)\approx117.9^\circ
}
$$

$$
\boxed{\vec{a}\times\vec{b}=(-10,7,9)}
$$

$$
\boxed{\text{Area}=\sqrt{230}\approx15.17}
$$

$$
\boxed{A\vec{a}=(3,-4,5)}
$$

$$
\boxed{\det A=1}
$$

$$
\boxed{\text{The transformation preserves orientation}.}
$$
