## Problem 1 – Vectors and linear transformations

### Problem statement

Given two vectors in three-dimensional space:

$$
\vec{a}=(2,-1,3), \qquad \vec{b}=(1,4,-2)
$$

and the matrix

$$
A=
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix},
$$

we need to:

1. calculate the lengths of the vectors $$|\vec{a}|$$ and $$|\vec{b}|$$,
2. determine the normalized vector $$\hat{a}=\dfrac{\vec{a}}{|\vec{a}|}$$,
3. calculate the dot product $$\vec{a}\cdot\vec{b}$$ and the angle between the vectors,
4. calculate the cross product $$\vec{a}\times\vec{b}$$ and the area of the parallelogram spanned by these vectors,
5. calculate $$A\vec{a}$$,
6. calculate $$\det A$$,
7. check whether the transformation preserves the orientation of space.

---

## Step 1. Lengths of the vectors

For a vector in three-dimensional space,

$$
|(x,y,z)|=\sqrt{x^2+y^2+z^2}.
$$

### Length of $$\vec{a}$$

Since

$$
\vec{a}=(2,-1,3),
$$

we have

$$
|\vec{a}|=\sqrt{2^2+(-1)^2+3^2}.
$$

Now calculate each square:

$$
2^2=4,\qquad (-1)^2=1,\qquad 3^2=9.
$$

So

$$
|\vec{a}|=\sqrt{4+1+9}=\sqrt{14}.
$$

Therefore,

$$
\boxed{|\vec{a}|=\sqrt{14}}.
$$

### Length of $$\vec{b}$$

Since

$$
\vec{b}=(1,4,-2),
$$

we have

$$
|\vec{b}|=\sqrt{1^2+4^2+(-2)^2}.
$$

Now calculate each square:

$$
1^2=1,\qquad 4^2=16,\qquad (-2)^2=4.
$$

So

$$
|\vec{b}|=\sqrt{1+16+4}=\sqrt{21}.
$$

Therefore,

$$
\boxed{|\vec{b}|=\sqrt{21}}.
$$

---

## Step 2. Normalized vector $$\hat{a}$$

The normalized vector is defined by

$$
\hat{a}=\frac{\vec{a}}{|\vec{a}|}.
$$

We already found that

$$
|\vec{a}|=\sqrt{14}.
$$

Thus,

$$
\hat{a}=\frac{(2,-1,3)}{\sqrt{14}}.
$$

Dividing each component by $$\sqrt{14}$$ gives

$$
\hat{a}=\left(\frac{2}{\sqrt{14}},\frac{-1}{\sqrt{14}},\frac{3}{\sqrt{14}}\right).
$$

Hence,

$$
\boxed{
\hat{a}=\left(\frac{2}{\sqrt{14}},-\frac{1}{\sqrt{14}},\frac{3}{\sqrt{14}}\right)
}.
$$

---

## Step 3. Dot product and the angle between the vectors

### Dot product

For two vectors

$$
\vec{a}=(a_1,a_2,a_3), \qquad \vec{b}=(b_1,b_2,b_3),
$$

their dot product is

$$
\vec{a}\cdot\vec{b}=a_1b_1+a_2b_2+a_3b_3.
$$

Substitute the given vectors:

$$
\vec{a}\cdot\vec{b}=2\cdot 1+(-1)\cdot 4+3\cdot(-2).
$$

Now calculate term by term:

$$
2\cdot 1=2,\qquad (-1)\cdot 4=-4,\qquad 3\cdot(-2)=-6.
$$

So

$$
\vec{a}\cdot\vec{b}=2-4-6=-8.
$$

Therefore,

$$
\boxed{\vec{a}\cdot\vec{b}=-8}.
$$

### Angle between the vectors

The angle $$\theta$$ between two vectors satisfies

$$
\cos\theta=\frac{\vec{a}\cdot\vec{b}}{|\vec{a}||\vec{b}|}.
$$

We already know that

$$
\vec{a}\cdot\vec{b}=-8,\qquad |\vec{a}|=\sqrt{14},\qquad |\vec{b}|=\sqrt{21}.
$$

Substitute into the formula:

$$
\cos\theta=\frac{-8}{\sqrt{14}\sqrt{21}}.
$$

Since

$$
\sqrt{14}\sqrt{21}=\sqrt{294},
$$

we obtain

$$
\cos\theta=\frac{-8}{\sqrt{294}}.
$$

Therefore,

$$
\boxed{\theta=\arccos\left(\frac{-8}{\sqrt{294}}\right)}.
$$

Approximate value:

$$
\sqrt{294}\approx 17.146,
$$

so

$$
\cos\theta\approx \frac{-8}{17.146}\approx -0.467.
$$

Hence,

$$
\theta\approx \arccos(-0.467)\approx 117.9^\circ.
$$

Thus,

$$
\boxed{\theta\approx 117.9^\circ}.
$$

---

## Step 4. Cross product and area of the parallelogram

### Cross product

For two vectors

$$
\vec{a}=(a_1,a_2,a_3), \qquad \vec{b}=(b_1,b_2,b_3),
$$

the cross product is

$$
\vec{a}\times\vec{b}=
\begin{pmatrix}
a_2b_3-a_3b_2 \\
a_3b_1-a_1b_3 \\
a_1b_2-a_2b_1
\end{pmatrix}.
$$

Substitute

$$
\vec{a}=(2,-1,3),\qquad \vec{b}=(1,4,-2).
$$

Now compute each component.

### First component

$$
a_2b_3-a_3b_2=(-1)(-2)-3\cdot 4=2-12=-10.
$$

### Second component

$$
a_3b_1-a_1b_3=3\cdot 1-2(-2)=3+4=7.
$$

### Third component

$$
a_1b_2-a_2b_1=2\cdot 4-(-1)\cdot 1=8+1=9.
$$

So,

$$
\vec{a}\times\vec{b}=(-10,7,9).
$$

Therefore,

$$
\boxed{\vec{a}\times\vec{b}=(-10,7,9)}.
$$

### Area of the parallelogram

The area of the parallelogram spanned by $$\vec{a}$$ and $$\vec{b}$$ is

$$
|\vec{a}\times\vec{b}|.
$$

So we calculate the length of $$(-10,7,9)$$:

$$
|\vec{a}\times\vec{b}|=\sqrt{(-10)^2+7^2+9^2}.
$$

Now compute:

$$
(-10)^2=100,\qquad 7^2=49,\qquad 9^2=81.
$$

Thus,

$$
|\vec{a}\times\vec{b}|=\sqrt{100+49+81}=\sqrt{230}.
$$

Hence, the area is

$$
\boxed{\sqrt{230}}.
$$

Approximate value:

$$
\sqrt{230}\approx 15.17.
$$

So,

$$
\boxed{\text{Area}\approx 15.17}.
$$

---

## Step 5. Calculate $$A\vec{a}$$

We are given

$$
A=
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix},
\qquad
\vec{a}=
\begin{pmatrix}
2\\
-1\\
3
\end{pmatrix}.
$$

Now multiply the matrix by the vector.

### First row

$$
2\cdot 2+1\cdot(-1)+0\cdot 3=4-1+0=3.
$$

### Second row

$$
0\cdot 2+1\cdot(-1)+(-1)\cdot 3=0-1-3=-4.
$$

### Third row

$$
1\cdot 2+0\cdot(-1)+1\cdot 3=2+0+3=5.
$$

Therefore,

$$
A\vec{a}=
\begin{pmatrix}
3\\
-4\\
5
\end{pmatrix}.
$$

So,

$$
\boxed{A\vec{a}=(3,-4,5)}.
$$

---

## Step 6. Calculate $$\det A$$

We compute the determinant by expanding along the first row:

$$
\det A=
\begin{vmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{vmatrix}.
$$

Using cofactor expansion:

$$
\det A
=
2
\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
-1
\begin{vmatrix}
0 & -1 \\
1 & 1
\end{vmatrix}
+0
\begin{vmatrix}
0 & 1 \\
1 & 0
\end{vmatrix}.
$$

Now calculate each minor.

### First minor

$$
\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
=1\cdot 1-(-1)\cdot 0=1.
$$

### Second minor

$$
\begin{vmatrix}
0 & -1 \\
1 & 1
\end{vmatrix}
=0\cdot 1-(-1)\cdot 1=1.
$$

So,

$$
\det A=2\cdot 1-1\cdot 1+0=2-1=1.
$$

Therefore,

$$
\boxed{\det A=1}.
$$

---

## Step 7. Check orientation preservation

A linear transformation preserves the orientation of space if

$$
\det A>0.
$$

It reverses the orientation if

$$
\det A<0.
$$

We found that

$$
\det A=1.
$$

Since

$$
1>0,
$$

the transformation preserves the orientation of space.

Therefore,

$$
\boxed{\text{The transformation preserves orientation.}}
$$

---

## Final answers

$$
\boxed{|\vec{a}|=\sqrt{14}}
$$

$$
\boxed{|\vec{b}|=\sqrt{21}}
$$

$$
\boxed{
\hat{a}=\left(\frac{2}{\sqrt{14}},-\frac{1}{\sqrt{14}},\frac{3}{\sqrt{14}}\right)
}
$$

$$
\boxed{\vec{a}\cdot\vec{b}=-8}
$$

$$
\boxed{\theta=\arccos\left(\frac{-8}{\sqrt{294}}\right)\approx 117.9^\circ}
$$

$$
\boxed{\vec{a}\times\vec{b}=(-10,7,9)}
$$

$$
\boxed{\text{Area of the parallelogram}=\sqrt{230}\approx 15.17}
$$

$$
\boxed{A\vec{a}=(3,-4,5)}
$$

$$
\boxed{\det A=1}
$$

$$
\boxed{\text{The transformation preserves orientation}}
$$
