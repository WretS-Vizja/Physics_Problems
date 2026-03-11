# Section 0: Mathematical Foundations
> This document contains solutions to the mathematical foundations problems used in the Physics Problems repository. The goal is to review the essential mathematical tools required for solving physics problems.
## 1. Vector Algebra

Given two vectors in 3D space: $\vec{a} = [2, 1, -3]$ and $\vec{b} = [4, -2, 1]$. Calculate:

a) The magnitude of each vector.

>**Problem**

> Find the magnitude (length) of vectors $\vec{a}$ and $\vec{b}$.

> **Idea**
>
> The magnitude of a vector in three-dimensional space is computed using the square root of the sum of the squares of its components.
>
> $$
> |\vec{v}| = \sqrt{v_x^2 + v_y^2 + v_z^2}
> $$

> **Step 1 – Compute the magnitude of $\vec{a}$**
>
> $$
> |\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2}
> $$

> **Step 2 – Square each component**
>
> $$
> 2^2 = 4
> $$
>
> $$
> 1^2 = 1
> $$
>
> $$
> (-3)^2 = 9
> $$

> **Step 3 – Sum the squares**
>
> $$
> 4 + 1 + 9 = 14
> $$

> **Step 4 – Take the square root**
>
> $$
> |\vec{a}| = \sqrt{14}
> $$

> **Step 5 – Compute the magnitude of $\vec{b}$**
>
> $$
> |\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2}
> $$

> **Step 6 – Square each component**
>
> $$
> 4^2 = 16
> $$
>
> $$
> (-2)^2 = 4
> $$
>
> $$
> 1^2 = 1
> $$

> **Step 7 – Sum the squares**
>
> $$
> 16 + 4 + 1 = 21
> $$

> **Step 8 – Take the square root**
>
> $$
> |\vec{b}| = \sqrt{21}
> $$

> **Result**
>
> $$
> |\vec{a}| = \sqrt{14}
> $$
>
> $$
> |\vec{b}| = \sqrt{21}
> $$
---

b) The dot product $\vec{a} \cdot \vec{b}$.

>**Problem**

> Find the dot product of vectors $\vec{a}$ and $\vec{b}$.

> **Idea**
>
> The dot product multiplies the corresponding components of the vectors and sums the results.
>
> $$
> \vec{a} \cdot \vec{b} =
> a_x b_x + a_y b_y + a_z b_z
> $$

> **Step 1 – Substitute the components**
>
> $$
> (2)(4) + (1)(-2) + (-3)(1)
> $$

> **Step 2 – Multiply the components**
>
> $$
> 8 - 2 - 3
> $$

> **Step 3 – Add the results**
>
> $$
> 3
> $$

> **Result**
>
> $$
> \vec{a} \cdot \vec{b} = 3
> $$

---
c) The cross product $\vec{a} \times \vec{b}$.

>**Problem**

> Find the cross product of the vectors $\vec{a}$ and $\vec{b}$.

> **Idea**
>
> The cross product produces a vector that is perpendicular to both vectors.  
> It can be computed using a determinant.

> **Step 1 – Write the determinant**
>
> $$
> \vec{a} \times \vec{b} =
> \begin{vmatrix}
> \hat{i} & \hat{j} & \hat{k} \\
> 2 & 1 & -3 \\
> 4 & -2 & 1
> \end{vmatrix}
> $$

> **Step 2 – Expand the determinant**
>
> $$
> \begin{aligned}
> \vec{a} \times \vec{b}
> &= \hat{i}(1\cdot1 - (-3)(-2)) \\
> &- \hat{j}(2\cdot1 - (-3)\cdot4) \\
> &+ \hat{k}(2\cdot(-2) - 1\cdot4)
> \end{aligned}
> $$

> **Step 3 – Compute each term**
>
> $$
> \begin{aligned}
> &= \hat{i}(1 - 6) \\
> &- \hat{j}(2 + 12) \\
> &+ \hat{k}(-4 - 4)
> \end{aligned}
> $$

> **Step 4 – Simplify**
>
> $$
> = -5\hat{i} - 14\hat{j} - 8\hat{k}
> $$

> **Result**
>
> $$
> \vec{a} \times \vec{b} = [-5,-14,-8] = -5\hat{i} -14\hat{j} -8\hat{k}
> $$

---

d) The angle between vectors $\vec{a}$ and $\vec{b}$.

>**Problem**

> Find the angle between vectors $\vec{a}$ and $\vec{b}$.

> **Idea**
>
> The angle between two vectors can be computed using the dot product formula.
>
> $$
> \cos\theta =
> \frac{\vec{a} \cdot \vec{b}}{|\vec{a}| |\vec{b}|}
> $$

> **Step 1 – Substitute the known values**
>
> $$
> \cos\theta =
> \frac{3}{\sqrt{14}\sqrt{21}}
> $$

> **Step 2 – Combine the square roots**
>
> $$
> \cos\theta =
> \frac{3}{\sqrt{294}}
> $$

> **Step 3 – Compute the angle**
>
> $$
> \theta =
> \arccos\left(\frac{3}{\sqrt{294}}\right)
> $$

> **Step 4 – Numerical value**
>
> $$
> \theta \approx 79.9^\circ
> $$

> **Result**
>
> The angle between the vectors is approximately
>
> $$
> \theta \approx 79.9^\circ
> $$
>
> The vectors form an **acute angle**.

---

## 2. Systems of Equations

> Find the values of $x$ and $y$ that satisfy both equations: $2x + 3y = 12$ and $x - y = 1$.

> **Problem**

> Solve the system of two linear equations for $x$ and $y$.

> **Idea**
>
> Use the substitution method: express one variable from the simpler equation and substitute it into the other.

> **Step 1 – Isolate $x$ from the second equation**
>
> $$
> x - y = 1 \implies x = y + 1
> $$

> **Step 2 – Substitute into the first equation**
>
> $$
> 2(y + 1) + 3y = 12
> $$

> **Step 3 – Expand**
>
> $$
> 2y + 2 + 3y = 12
> $$

> **Step 4 – Collect like terms**
>
> $$
> 5y = 10
> $$

> **Step 5 – Solve for $y$**
>
> $$
> y = 2
> $$

> **Step 6 – Solve for $x$**
>
> $$
> x = y + 1 = 2 + 1 = 3
> $$

> **Result**
>
> $$
> x = 3, \quad y = 2
> $$

---

## 3. Proportionality

Consider the Universal Law of Gravitation: $F = G \frac{m_1 m_2}{r^2}$, where $F$ is the gravitational force between two masses $m_1$ and $m_2$, $r$ is the distance between their centers, and $G$ is the gravitational constant. Determine the factor by which the force $F$ changes if the distance $r$ is *doubled* and both masses ($m_1$ and $m_2$) are *halved*.

> **Problem**

> Find the new force $F'$ in terms of the original force $F$ after applying the given changes.

> **Idea**
>
> Substitute the transformed quantities into the formula and compare with the original.

> **Step 1 – Write the original force**
>
> $$
> F = G \frac{m_1 m_2}{r^2}
> $$

> **Step 2 – Apply the changes**
>
> $$
> m_1' = \frac{m_1}{2}, \quad m_2' = \frac{m_2}{2}, \quad r' = 2r
> $$

> **Step 3 – Write the new force**
>
> $$
> F' = G \frac{\left(\dfrac{m_1}{2}\right)\left(\dfrac{m_2}{2}\right)}{(2r)^2}
> $$

> **Step 4 – Simplify the numerator**
>
> $$
> F' = G \frac{\dfrac{m_1 m_2}{4}}{4r^2}
> $$

> **Step 5 – Simplify the full expression**
>
> $$
> F' = G \frac{m_1 m_2}{16 r^2}
> $$

> **Step 6 – Compare with original**
>
> $$
> F' = \frac{1}{16} \cdot G \frac{m_1 m_2}{r^2} = \frac{F}{16}
> $$

> **Result**
>
> The gravitational force decreases by a factor of **16**.
>
> $$
> F' = \frac{F}{16}
> $$

---

## 4. Rearranging Formulas

The formula for the period of a simple pendulum is $T = 2\pi \sqrt{\frac{L}{g}}$. Rearrange the equation give a formula for $g$ (acceleration due to gravity).

> **Problem**

> Isolate $g$ (acceleration due to gravity) from the pendulum period formula.

> **Idea**
>
> Algebraically rearrange by squaring both sides and isolating $g$.

> **Step 1 – Square both sides**
>
> $$
> T^2 = 4\pi^2 \frac{L}{g}
> $$

> **Step 2 – Multiply both sides by $g$**
>
> $$
> T^2 \cdot g = 4\pi^2 L
> $$

> **Step 3 – Divide both sides by $T^2$**
>
> $$
> g = \frac{4\pi^2 L}{T^2}
> $$

> **Result**
>
> $$
> g = \frac{4\pi^2 L}{T^2}
> $$

---

## 5. Trigonometry

A vector $\vec{A}$ has a magnitude of $15$ and makes an angle of $\theta = 60^\circ$ with the horizontal axis. Calculate its horizontal and vertical components.
> **Problem**

> Find the $x$ and $y$ components of vector $\vec{A}$.

> **Idea**
>
> The components of a vector are found using trigonometric projections.
>
> $$
> A_x = |\vec{A}|\cos\theta, \quad A_y = |\vec{A}|\sin\theta
> $$

> **Step 1 – Compute the horizontal component**
>
> $$
> A_x = 15 \cos 60^\circ
> $$

> **Step 2 – Substitute the known value $\cos 60^\circ = 0.5$**
>
> $$
> A_x = 15 \times 0.5 = 7.5
> $$

> **Step 3 – Compute the vertical component**
>
> $$
> A_y = 15 \sin 60^\circ
> $$

> **Step 4 – Substitute the known value $\sin 60^\circ = \dfrac{\sqrt{3}}{2}$**
>
> $$
> A_y = 15 \times \frac{\sqrt{3}}{2} = \frac{15\sqrt{3}}{2} \approx 12.99
> $$

> **Result**
>
> $$
> A_x = 7.5, \quad A_y = \frac{15\sqrt{3}}{2} \approx 12.99
> $$

---

## 6. Function Analysis

Consider the function $f(x) = 3x^2 - 12x + 7$. Identify any local maxima or minima.
> **Problem**

> Find the local extrema of the function $f(x)$.

> **Idea**
>
> To find extrema, take the first derivative, set it equal to zero, and use the second derivative to classify the critical point.

> **Step 1 – Compute the first derivative**
>
> $$
> f'(x) = 6x - 12
> $$

> **Step 2 – Set $f'(x) = 0$ and solve**
>
> $$
> 6x - 12 = 0 \implies x = 2
> $$

> **Step 3 – Compute the second derivative**
>
> $$
> f''(x) = 6
> $$

> **Step 4 – Classify the critical point**
>
> Since $f''(2) = 6 > 0$, the function is concave up at $x = 2$, so it is a **local minimum**.

> **Step 5 – Find the function value at the minimum**
>
> $$
> f(2) = 3(4) - 12(2) + 7 = 12 - 24 + 7 = -5
> $$

> **Result**
>
> The function has a **local minimum** at $(2,\ -5)$.  
> There is no local maximum (the parabola opens upward).

---

## 7. Logic & Series

A bicycle is 10 meters from a wall and moves towards it at a constant speed of $1\text{ m/s}$. A fly starts from the bicycle's front wheel and flies towards the wall at $2\text{ m/s}$. When it hits the wall, it instantly turns back and flies to the bicycle, and so on. What is the total distance the fly travels before being crushed?

> **Problem**

> Find the total distance traveled by the fly before the bicycle reaches the wall.

> **Idea**
>
> Instead of summing the infinite back-and-forth trips, use a time argument: the fly travels for the same total duration as the bicycle's journey.

> **Step 1 – Find the time until the bicycle reaches the wall**
>
> $$
> t = \frac{d}{v} = \frac{10\ \text{m}}{1\ \text{m/s}} = 10\ \text{s}
> $$

> **Step 2 – Compute the total distance of the fly**
>
> The fly travels at $2\ \text{m/s}$ for the entire $10\ \text{s}$.
>
> $$
> d_{\text{fly}} = v_{\text{fly}} \times t = 2 \times 10 = 20\ \text{m}
> $$

> **Result**
>
> The fly travels a total distance of $\mathbf{20\ \text{m}}$.

---

## 8. Definite Integrals

Calculate the area under the curve of the function $f(x) = \sin(x)$ from $x=0$ to $x=\pi$.

> **Problem**

> Evaluate the definite integral $\displaystyle\int_0^{\pi} \sin(x)\ dx$.

> **Idea**
>
> Use the antiderivative of $\sin(x)$, which is $-\cos(x)$, and apply the fundamental theorem of calculus.

> **Step 1 – Write the integral**
>
> $$
> \int_0^{\pi} \sin(x)\ dx
> $$

> **Step 2 – Find the antiderivative**
>
> $$
> \int \sin(x)\ dx = -\cos(x)
> $$

> **Step 3 – Evaluate at the bounds**
>
> $$
> \Big[-\cos(x)\Big]_0^{\pi} = -\cos(\pi) - (-\cos(0))
> $$

> **Step 4 – Substitute known values**
>
> $$
> \cos(\pi) = -1, \quad \cos(0) = 1
> $$
>
> $$
> = -(-1) + 1 = 1 + 1 = 2
> $$

> **Result**
>
> $$
> \int_0^{\pi} \sin(x)\ dx = 2
> $$
>
> The area under the curve is $\mathbf{2}$ square units.

---

## 9. Optimization Problem

A rectangle is under the curve $y = 3 - x^2$ in the first quadrant. What are the dimensions of the rectangle with the maximum area?
> **Solution:**
>
> Area $A = x \cdot y = x(3 - x^2) = 3x - x^3$
>
> 1. Find the derivative of the area:
> $$A'(x) = 3 - 3x^2$$
>
> 2. Set $A'(x) = 0$:
> $$3 - 3x^2 = 0 \Rightarrow x^2 = 1 \Rightarrow \mathbf{x = 1}$$
>
> 3. Calculate $y$:
> $$y = 3 - (1)^2 = \mathbf{2}$$
> **Dimensions:** $1 \times 2$.

## 10. Infinite Series

Determine the final position of an ant that starts at the origin and moves according to the following pattern: 1 m east, 1/2 m north, 1/3 m west, 1/4 m south, 1/5 m east, and so on.
> **Solution:**
>
> **x-coordinate (East/West):**
> $$x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \dots = \sum_{n=0}^{\infty} \frac{(-1)^n}{2n+1} = \mathbf{\frac{\pi}{4}}$$
>
> **y-coordinate (North/South):**
> $$y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \dots = \frac{1}{2} \left( 1 - \frac{1}{2} + \frac{1}{3} - \dots \right) = \frac{1}{2} \ln(2) = \mathbf{\ln(\sqrt{2})}$$
>
> **Final Position:** $(\frac{\pi}{4}, \ln\sqrt{2}) \approx (0.785, 0.347)$
