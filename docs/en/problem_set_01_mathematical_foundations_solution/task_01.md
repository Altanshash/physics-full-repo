# Problem 1 – Vectors and linear transformations

Please write down all calculation steps, not just the final results.

## Given

We are given two vectors in three-dimensional space:

$$
\vec{a} = (2, -1, 3), \qquad \vec{b} = (1, 4, -2)
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

## 1. Lengths of the vectors $|\vec a|$ and $|\vec b|$

### Length of $\vec a$

$$
|\vec a| = \sqrt{2^2 + (-1)^2 + 3^2}
$$

$$
|\vec a| = \sqrt{4 + 1 + 9} = \sqrt{14}
$$

### Length of $\vec b$

$$
|\vec b| = \sqrt{1^2 + 4^2 + (-2)^2}
$$

$$
|\vec b| = \sqrt{1 + 16 + 4} = \sqrt{21}
$$

### Answer

$$
|\vec a| = \sqrt{14}, \qquad |\vec b| = \sqrt{21}
$$

---

## 2. Normalized vector of $\vec a$

The normalized vector is

$$
\hat a = \frac{\vec a}{|\vec a|}
$$

Substitute $\vec a = (2,-1,3)$ and $|\vec a| = \sqrt{14}$:

$$
\hat a = \left( \frac{2}{\sqrt{14}}, \frac{-1}{\sqrt{14}}, \frac{3}{\sqrt{14}} \right)
$$

### Answer

$$
\hat a = \left( \frac{2}{\sqrt{14}}, -\frac{1}{\sqrt{14}}, \frac{3}{\sqrt{14}} \right)
$$

---

## 3. Dot product $\vec a \cdot \vec b$ and the angle between the vectors

### Dot product

$$
\vec a \cdot \vec b = 2\cdot1 + (-1)\cdot4 + 3\cdot(-2)
$$

$$
\vec a \cdot \vec b = 2 - 4 - 6 = -8
$$

### Angle formula

$$
\vec a \cdot \vec b = |\vec a| |\vec b| \cos\theta
$$

So,

$$
\cos\theta = \frac{\vec a \cdot \vec b}{|\vec a||\vec b|}
$$

Substitute the values:

$$
\cos\theta = \frac{-8}{\sqrt{14}\sqrt{21}}
$$

$$
\cos\theta = \frac{-8}{\sqrt{294}}
$$

Thus,

$$
\theta = \cos^{-1}\left(\frac{-8}{\sqrt{294}}\right)
$$

Approximate value:

$$
\sqrt{294} \approx 17.146
$$

$$
\cos\theta \approx \frac{-8}{17.146} \approx -0.467
$$

$$
\theta \approx \cos^{-1}(-0.467) \approx 117.9^\circ
$$

### Answer

$$
\vec a \cdot \vec b = -8
$$

$$
\theta = \cos^{-1}\left(\frac{-8}{\sqrt{294}}\right) \approx 117.9^\circ
$$

---

## 4. Cross product $\vec a \times \vec b$ and the area of the parallelogram

### Cross product

$$
\vec a \times \vec b =
\begin{vmatrix}
\mathbf i & \mathbf j & \mathbf k \\
2 & -1 & 3 \\
1 & 4 & -2
\end{vmatrix}
$$

Expand by the first row:

$$
\vec a \times \vec b =
\mathbf i
\begin{vmatrix}
-1 & 3 \\
4 & -2
\end{vmatrix}
-
\mathbf j
\begin{vmatrix}
2 & 3 \\
1 & -2
\end{vmatrix}
+
\mathbf k
\begin{vmatrix}
2 & -1 \\
1 & 4
\end{vmatrix}
$$

Now calculate each determinant.

### $\mathbf i$-component

$$
(-1)(-2) - (3)(4) = 2 - 12 = -10
$$

### $\mathbf j$-component

$$
(2)(-2) - (3)(1) = -4 - 3 = -7
$$

Because of the minus sign before $\mathbf j$:

$$
-\mathbf j(-7) = 7\mathbf j
$$

### $\mathbf k$-component

$$
(2)(4) - (-1)(1) = 8 + 1 = 9
$$

So,

$$
\vec a \times \vec b = (-10, 7, 9)
$$

### Area of the parallelogram

The area is the magnitude of the cross product:

$$
|\vec a \times \vec b| = \sqrt{(-10)^2 + 7^2 + 9^2}
$$

$$
|\vec a \times \vec b| = \sqrt{100 + 49 + 81}
$$

$$
|\vec a \times \vec b| = \sqrt{230}
$$

### Answer

$$
\vec a \times \vec b = (-10, 7, 9)
$$

$$
\text{Area of the parallelogram} = \sqrt{230}
$$

---

## 5. Calculate $A\vec a$

We multiply the matrix $A$ by the vector $\vec a$:

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

Now calculate row by row.

### First component

$$
2\cdot2 + 1\cdot(-1) + 0\cdot3 = 4 - 1 + 0 = 3
$$

### Second component

$$
0\cdot2 + 1\cdot(-1) + (-1)\cdot3 = 0 - 1 - 3 = -4
$$

### Third component

$$
1\cdot2 + 0\cdot(-1) + 1\cdot3 = 2 + 0 + 3 = 5
$$

So,

$$
A\vec a =
\begin{pmatrix}
3 \\
-4 \\
5
\end{pmatrix}
$$

### Answer

$$
A\vec a = (3, -4, 5)
$$

---

## 6. Calculate $\det(A)$

$$
A =
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}
$$

Expand along the first row:

$$
\det(A) =
2\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
-
1\begin{vmatrix}
0 & -1 \\
1 & 1
\end{vmatrix}
+
0\begin{vmatrix}
0 & 1 \\
1 & 0
\end{vmatrix}
$$

Now compute:

### First minor

$$
\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
= 1\cdot1 - (-1)\cdot0 = 1
$$

### Second minor

$$
\begin{vmatrix}
0 & -1 \\
1 & 1
\end{vmatrix}
= 0\cdot1 - (-1)\cdot1 = 1
$$

Thus,

$$
\det(A) = 2(1) - 1(1) + 0 = 1
$$

### Answer

$$
\det(A) = 1
$$

---

## 7. Does the transformation preserve orientation?

A linear transformation preserves orientation if

$$
\det(A) > 0
$$

From the previous calculation,

$$
\det(A) = 1 > 0
$$

Therefore, the transformation **does preserve orientation**.

### Answer

Yes, the transformation preserves orientation because

$$
\det(A) = 1 > 0
$$

---

## Final Answers

$$
|\vec a| = \sqrt{14}, \qquad |\vec b| = \sqrt{21}
$$

$$
\hat a = \left( \frac{2}{\sqrt{14}}, -\frac{1}{\sqrt{14}}, \frac{3}{\sqrt{14}} \right)
$$

$$
\vec a \cdot \vec b = -8
$$

$$
\theta = \cos^{-1}\left(\frac{-8}{\sqrt{294}}\right) \approx 117.9^\circ
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
