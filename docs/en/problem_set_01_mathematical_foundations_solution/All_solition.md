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

## Problem 2 – Parametric trajectory

$$
\vec r(t) = (t^2,\sin t,5)
$$

Velocity:
$$
\vec v(t) = \frac{d\vec r}{dt} = (2t,\cos t,0)
$$

Acceleration:
$$
\vec a(t) = (2,-\sin t,0)
$$

Speed at $t=1$:
$$
|\vec v(1)| = \sqrt{4 + \cos^2 1}
$$

Dot product:
$$
\vec v \cdot \vec a = 4t - \sin t \cos t
$$

Cross product:
$$
\vec v \times \vec a = (0,0,-2t\sin t - 2\cos t)
$$

---

## Problem 3 – Integration of motion

### A)

$$
\vec v(t) = (2t,3,-e^{-t}), \quad \vec r(0)=(0,1,2)
$$

$$
\vec r(t) = \vec r(0) + \int_0^t \vec v(\tau)d\tau
$$

$$
= (0,1,2) + (t^2,3t,e^{-t}-1)
$$

$$
= (t^2,1+3t,1+e^{-t})
$$

Acceleration:
$$
\vec a(t) = (2,0,e^{-t})
$$

---

### B)

$$
\vec a(t) = (4,-\sin t,0)
$$

$$
\vec v(t) = (1,0,2) + (4t,1-\cos t,0)
$$

$$
= (1+4t,1-\cos t,2)
$$

$$
\vec r(t) = (0,0,0) + \int_0^t \vec v(\tau)d\tau
$$

$$
= (t+2t^2, t-\sin t, 2t)
$$

---

## Problem 4 – Geometry of curves

### A)

$$
x=R\cos t,\quad y=R\sin t
$$

$$
x^2+y^2=R^2
$$

Velocity:
$$
\vec v=(-R\sin t,R\cos t)
$$

$$
|\vec v|=R
$$

---

### B)

$$
x=a\cos t,\quad y=b\sin t
$$

$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
$$

Ellipse.

---

### C)

$$
x=t,\quad y=t^2
$$

$$
y=x^2
$$

Parabola.

---

### D)

$$
x=\cosh t,\quad y=\sinh t
$$

$$
x^2-y^2=1
$$

Hyperbola.

---

## Problem 5 – Curvature of ellipse

$$
x=a\cos t,\quad y=b\sin t
$$

$$
\vec v=(-a\sin t,b\cos t)
$$

$$
\vec a=(-a\cos t,-b\sin t)
$$

Radius of curvature at $t=0$:
$$
R=\frac{a^2}{b}
$$

For $a=b$:
$$
R=a
$$

---

## Problem 6 – Curve length

$$
x=t,\quad y=t^2
$$

$$
\vec v=(1,2t)
$$

$$
|\vec v|=\sqrt{1+4t^2}
$$

$$
s=\int_0^1 \sqrt{1+4t^2}\,dt
$$

Numerical integration required.

---

## Problem 7 – Work

$$
\vec F=(y,2x),\quad x=t,\;y=t^2
$$

$$
\vec v=(1,2t)
$$

$$
\vec F=(t^2,2t)
$$

$$
W=\int_0^1 (t^2,2t)\cdot(1,2t)\,dt
$$

$$
=\int_0^1 5t^2 dt = \frac{5}{3}
$$

---

## Problem 8 – First-order ODE

$$
\frac{dy}{dt}=-ky
$$

$$
y(t)=Ce^{-kt}
$$

---

## Problem 9 – Harmonic oscillator

$$
\frac{d^2x}{dt^2}+\omega^2 x=0
$$

$$
x(t)=A\cos(\omega t)+B\sin(\omega t)
$$

---

## Problem 10 – Angular momentum

$$
\vec r=(R\cos\omega t,R\sin\omega t,0)
$$

$$
\vec v=(-R\omega\sin\omega t,R\omega\cos\omega t,0)
$$

$$
\vec L=m\vec r\times\vec v=(0,0,mR^2\omega)
$$

$$
|\vec L|=mR^2\omega
$$

Constant and perpendicular to plane of motion.