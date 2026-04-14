# Problem 1 – Vectors and linear transformations

## Given

We are given the vectors

$$
\vec a = (2, -1, 3), \qquad \vec b = (1, 4, -2)
$$

and the matrix

$$
A =
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}
$$

---

## 1. Lengths of the vectors

For $\vec a = (2, -1, 3)$:

$$
|\vec a| = \sqrt{2^2 + (-1)^2 + 3^2}
$$

$$
|\vec a| = \sqrt{4 + 1 + 9} = \sqrt{14}
$$

For $\vec b = (1, 4, -2)$:

$$
|\vec b| = \sqrt{1^2 + 4^2 + (-2)^2}
$$

$$
|\vec b| = \sqrt{1 + 16 + 4} = \sqrt{21}
$$

Therefore,

$$
|\vec a| = \sqrt{14}, \qquad |\vec b| = \sqrt{21}
$$

---

## 2. Normalized vector of $\vec a$

The normalized vector is

$$
\hat a = \frac{\vec a}{|\vec a|}
$$

Substitute $\vec a = (2, -1, 3)$ and $|\vec a| = \sqrt{14}$:

$$
\hat a = \left( \frac{2}{\sqrt{14}}, \frac{-1}{\sqrt{14}}, \frac{3}{\sqrt{14}} \right)
$$

So,

$$
\hat a = \left( \frac{2}{\sqrt{14}}, -\frac{1}{\sqrt{14}}, \frac{3}{\sqrt{14}} \right)
$$

---

## 3. Dot product and angle between the vectors

The dot product is

$$
\vec a \cdot \vec b = 2 \cdot 1 + (-1) \cdot 4 + 3 \cdot (-2)
$$

$$
\vec a \cdot \vec b = 2 - 4 - 6 = -8
$$

Now use the formula

$$
\vec a \cdot \vec b = |\vec a| |\vec b| \cos \theta
$$

So,

$$
\cos \theta = \frac{\vec a \cdot \vec b}{|\vec a||\vec b|}
$$

Substitute the known values:

$$
\cos \theta = \frac{-8}{\sqrt{14}\sqrt{21}} = \frac{-8}{\sqrt{294}}
$$

Hence,

$$
\theta = \cos^{-1} \left( \frac{-8}{\sqrt{294}} \right)
$$

Approximate value:

$$
\theta \approx 117.9^\circ
$$

Therefore,

$$
\vec a \cdot \vec b = -8
$$

and

$$
\theta = \cos^{-1} \left( \frac{-8}{\sqrt{294}} \right) \approx 117.9^\circ
$$

---

## 4. Cross product and area of the parallelogram

Use the coordinate formula for the cross product:

For

$$
\vec a = (a_1, a_2, a_3), \qquad \vec b = (b_1, b_2, b_3)
$$

we have

$$
\vec a \times \vec b =
(a_2b_3 - a_3b_2,\; a_3b_1 - a_1b_3,\; a_1b_2 - a_2b_1)
$$

Now substitute

$$
\vec a = (2, -1, 3), \qquad \vec b = (1, 4, -2)
$$

### First component

$$
a_2b_3 - a_3b_2 = (-1)(-2) - (3)(4) = 2 - 12 = -10
$$

### Second component

$$
a_3b_1 - a_1b_3 = (3)(1) - (2)(-2) = 3 + 4 = 7
$$

### Third component

$$
a_1b_2 - a_2b_1 = (2)(4) - (-1)(1) = 8 + 1 = 9
$$

Therefore,

$$
\vec a \times \vec b = (-10, 7, 9)
$$

The area of the parallelogram is the magnitude of the cross product:

$$
|\vec a \times \vec b| = \sqrt{(-10)^2 + 7^2 + 9^2}
$$

$$
|\vec a \times \vec b| = \sqrt{100 + 49 + 81}
$$

$$
|\vec a \times \vec b| = \sqrt{230}
$$

So,

$$
\vec a \times \vec b = (-10, 7, 9)
$$

and

$$
\text{Area} = \sqrt{230}
$$

---

## 5. Calculate $A\vec a$

We multiply the matrix by the vector:

$$
A\vec a =
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
2 \\
-1 \\
3
\end{pmatrix}
$$

Now compute each row.

### First component

$$
2 \cdot 2 + 1 \cdot (-1) + 0 \cdot 3 = 4 - 1 + 0 = 3
$$

### Second component

$$
0 \cdot 2 + 1 \cdot (-1) + (-1) \cdot 3 = -1 - 3 = -4
$$

### Third component

$$
1 \cdot 2 + 0 \cdot (-1) + 1 \cdot 3 = 2 + 3 = 5
$$

Therefore,

$$
A\vec a =
\begin{pmatrix}
3 \\
-4 \\
5
\end{pmatrix}
$$

So,

$$
A\vec a = (3, -4, 5)
$$

---

## 6. Calculate $\det(A)$

We use expansion along the first row:

$$
A =
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}
$$

So,

$$
\det(A) =
2 \cdot
\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
-
1 \cdot
\begin{vmatrix}
0 & -1 \\
1 & 1
\end{vmatrix}
+
0 \cdot
\begin{vmatrix}
0 & 1 \\
1 & 0
\end{vmatrix}
$$

Now compute the $2 \times 2$ determinants.

First:

$$
\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
= 1 \cdot 1 - (-1) \cdot 0 = 1
$$

Second:

$$
\begin{vmatrix}
0 & -1 \\
1 & 1
\end{vmatrix}
= 0 \cdot 1 - (-1) \cdot 1 = 1
$$

Third term is multiplied by $0$, so it is just $0$.

Therefore,

$$
\det(A) = 2 \cdot 1 - 1 \cdot 1 + 0 = 2 - 1 = 1
$$

So,

$$
\det(A) = 1
$$

---

## 7. Orientation of the transformation

A linear transformation preserves orientation if its determinant is positive.

Since

$$
\det(A) = 1 > 0
$$

the transformation preserves orientation.

---

## Final answers

$$
|\vec a| = \sqrt{14}
$$

$$
|\vec b| = \sqrt{21}
$$

$$
\hat a = \left( \frac{2}{\sqrt{14}}, -\frac{1}{\sqrt{14}}, \frac{3}{\sqrt{14}} \right)
$$

$$
\vec a \cdot \vec b = -8
$$

$$
\theta = \cos^{-1} \left( \frac{-8}{\sqrt{294}} \right) \approx 117.9^\circ
$$

$$
\vec a \times \vec b = (-10, 7, 9)
$$

$$
\text{Area} = \sqrt{230}
$$

$$
A\vec a = (3, -4, 5)
$$

$$
\det(A) = 1
$$

The transformation preserves orientation.
