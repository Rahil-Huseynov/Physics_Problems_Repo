
## Problem 1 – Vectors and linear transformations

Given:
$$
\vec a = (2,-1,3), \qquad
\vec b = (1,4,-2)
$$

### Lengths of vectors

$$
|\vec a| = \sqrt{2^2 + (-1)^2 + 3^2} = \sqrt{14}
$$

$$
|\vec b| = \sqrt{1^2 + 4^2 + (-2)^2} = \sqrt{21}
$$

---

### Normalized vector

$$
\hat a = \frac{\vec a}{|\vec a|} = \frac{1}{\sqrt{14}}(2,-1,3)
$$

---

### Dot product and angle

$$
\vec a \cdot \vec b = 2\cdot1 + (-1)\cdot4 + 3\cdot(-2) = -8
$$

$$
\cos\theta = \frac{\vec a\cdot\vec b}{|\vec a||\vec b|}
= \frac{-8}{\sqrt{14}\sqrt{21}}
$$

$$
\theta = \arccos\!\left(\frac{-8}{\sqrt{294}}\right)
$$

---

### Cross product

$$
\vec a \times \vec b =
\begin{vmatrix}
\hat i & \hat j & \hat k \\
2 & -1 & 3 \\
1 & 4 & -2
\end{vmatrix}
$$

$$
= (-10,7,9)
$$

Area of parallelogram:
$$
|\vec a \times \vec b| = \sqrt{(-10)^2 + 7^2 + 9^2} = \sqrt{230}
$$

---

### Matrix

$$
A =
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}
$$

Compute:
$$
A\vec a =
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
2 \\ -1 \\ 3
\end{pmatrix}
=
\begin{pmatrix}
3 \\ -4 \\ 5
\end{pmatrix}
$$

Determinant:
$$
\det A =
\begin{vmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{vmatrix}
= 1
$$

Since $\det A > 0$, the transformation preserves orientation.

---
