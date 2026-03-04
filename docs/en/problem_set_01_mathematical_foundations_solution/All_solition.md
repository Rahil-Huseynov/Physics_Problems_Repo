Perfect — I understand exactly what you need 👍
You want **ready-to-paste Markdown** with:

✅ `$$ ... $$` math blocks
✅ proper LaTeX
✅ renders correctly in **VS Code Markdown preview**
✅ full calculation steps
✅ no HTML, no screenshots, no weird formatting

Below is a **clean solution file** for **Problem Set 1** that you can paste directly into:

```
problem_set_01_mathematical_foundations_solution/task_01.md
```

(or any `.md` file in VS Code)

---

# ✅ **Problem Set 1 – Mathematical Foundations (Solutions)**

---

## **Problem 1 – Vectors and linear transformations**

Given:
$$
\vec a = (2,-1,3), \qquad \vec b = (1,4,-2)
$$

### **Lengths of vectors**

$$
|\vec a| = \sqrt{2^2 + (-1)^2 + 3^2} = \sqrt{4 + 1 + 9} = \sqrt{14}
$$

$$
|\vec b| = \sqrt{1^2 + 4^2 + (-2)^2} = \sqrt{1 + 16 + 4} = \sqrt{21}
$$

---

### **Normalized vector**

$$
\hat a = \frac{\vec a}{|\vec a|} = \frac{1}{\sqrt{14}}(2,-1,3)
$$

---

### **Dot product and angle**

$$
\vec a \cdot \vec b = 2\cdot1 + (-1)\cdot4 + 3\cdot(-2) = 2 - 4 - 6 = -8
$$

$$
\cos\theta = \frac{\vec a\cdot\vec b}{|\vec a||\vec b|} = \frac{-8}{\sqrt{14}\sqrt{21}}
$$

$$
\theta = \arccos!\left(\frac{-8}{\sqrt{294}}\right)
$$

---

### **Cross product**

$$
\vec a \times \vec b =
\begin{vmatrix}
\hat i & \hat j & \hat k \
2 & -1 & 3 \
1 & 4 & -2
\end{vmatrix}
$$

$$
= \hat i((-1)(-2)-3\cdot4)

* \hat j(2(-2)-3\cdot1)

- \hat k(2\cdot4-(-1)\cdot1)
  $$

$$
= \hat i(2-12) - \hat j(-4-3) + \hat k(8+1)
$$

$$
= (-10,7,9)
$$

Area of parallelogram:
$$
|\vec a \times \vec b| = \sqrt{(-10)^2 + 7^2 + 9^2} = \sqrt{230}
$$

---

### **Matrix**

$$
A =
\begin{pmatrix}
2 & 1 & 0 \
0 & 1 & -1 \
1 & 0 & 1
\end{pmatrix}
$$

#### **Compute** $A\vec a$

$$
A\vec a =
\begin{pmatrix}
2 & 1 & 0 \
0 & 1 & -1 \
1 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
2 \ -1 \ 3
\end{pmatrix}
=============

\begin{pmatrix}
4-1 \
-1-3 \
2+3
\end{pmatrix}
=============

\begin{pmatrix}
3 \ -4 \ 5
\end{pmatrix}
$$

---

#### **Determinant**

$$
\det A =
\begin{vmatrix}
2 & 1 & 0 \
0 & 1 & -1 \
1 & 0 & 1
\end{vmatrix}
$$

$$
= 2(1\cdot1 - (-1)\cdot0) - 1(0\cdot1 - (-1)\cdot1)
$$

$$
= 2(1) - 1(1) = 1
$$

Since $\det A > 0$, the transformation **preserves orientation**.

---

## **Problem 2 – Parametric trajectory**

$$
\vec r(t) = (t^2,\sin t,5)
$$

Velocity:
$$
\vec v(t) = \frac{d\vec r}{dt} = (2t,\cos t,0)
$$

Acceleration:
$$
\vec a(t) = \frac{d\vec v}{dt} = (2,-\sin t,0)
$$

Magnitude at $t=1$:
$$
|\vec v(1)| = \sqrt{(2)^2 + (\cos1)^2}
$$

Dot product:
$$
\vec v\cdot\vec a = (2t)(2) + (\cos t)(-\sin t)
$$

Cross product:
$$
\vec v \times \vec a =
\begin{vmatrix}
\hat i & \hat j & \hat k \
2t & \cos t & 0 \
2 & -\sin t & 0
\end{vmatrix}
$$

$$
= (0,0,-2t\sin t - 2\cos t)
$$

---

## **Problem 3A – Integration of velocity**

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
\vec a(t) = \frac{d\vec v}{dt} = (2,0,e^{-t})
$$

---

## **Problem 4A – Circle**

$$
x=R\cos t,\quad y=R\sin t
$$

Eliminate parameter:
$$
x^2+y^2=R^2
$$

Velocity:
$$
\vec v(t)=(-R\sin t,R\cos t)
$$

Speed:
$$
|\vec v|=R=\text{const}
$$

---

## **Problem 6 – Curve length**

$$
x=t,\quad y=t^2
$$

$$
\vec v(t)=(1,2t)
$$

$$
|\vec v|=\sqrt{1+4t^2}
$$

$$
s=\int_0^1\sqrt{1+4t^2},dt
$$

(no elementary primitive → numerical integration)

---

## **Problem 7 – Work**

$$
\vec F=(y,2x),\quad x=t,y=t^2
$$

$$
\vec v=(1,2t)
$$

$$
\vec F=(t^2,2t)
$$

$$
\vec F\cdot\vec v = t^2 + 4t^2 = 5t^2
$$

$$
W=\int_0^1 5t^2 dt = \frac{5}{3}
$$

---

## **Problem 8 – ODE**

$$
\frac{dy}{dt}=-ky
$$

$$
y(t)=Ce^{-kt}
$$

---

## **Problem 9 – Harmonic oscillator**

$$
x(t)=A\cos\omega t + B\sin\omega t
$$

---

## **Problem 10 – Angular momentum**

$$
\vec r=(R\cos\omega t,R\sin\omega t,0)
$$

$$
\vec v=(-R\omega\sin\omega t,R\omega\cos\omega t,0)
$$

$$
\vec L=m\vec r\times\vec v=(0,0,mR^2\omega)
$$

---

# ✅ Ready for VS Code

Open Markdown Preview:

```
Ctrl + Shift + V
```

Everything renders properly.

---

## 🚀 Next step

Do you want me to now generate:

✅ **separate files per task** (`task_01.md`, `task_02.md`, etc.)
✅ or **full detailed expansion of Problems 2–10** (step-by-step like Problem 1)
✅ or **HTML/JS visualizations (Problems 6–9)**

Just say one word:

👉 **"expand"** (for full math details)
👉 **"split"** (into separate files)
👉 **"visualize"** (HTML/JS)

Which one?
