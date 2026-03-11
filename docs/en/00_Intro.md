# Section 0: Mathematical Foundations
> This document contains solutions to the mathematical foundations problems used in the Physics Problems repository. The goal is to review the essential mathematical tools required for solving physics problems.
## 1. Vector Algebra

Given two vectors in 3D space: $\vec{a} = [2, 1, -3]$ and $\vec{b} = [4, -2, 1]$. Calculate:

a) The magnitude of each vector.
**Problem**

Find the magnitude (length) of vectors $\vec{a}$ and $\vec{b}$.

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
**Problem**

Find the dot product of vectors $\vec{a}$ and $\vec{b}$.

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
**Problem**

Find the cross product of the vectors $\vec{a}$ and $\vec{b}$.

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
> \vec{a} \times \vec{b} &=
> \hat{i}(1\cdot1 - (-3)(-2)) \\
> &\quad - \hat{j}(2\cdot1 - (-3)\cdot4) \\
> &\quad + \hat{k}(2\cdot(-2) - 1\cdot4)
> \end{aligned}
> $$

> **Step 3 – Compute each term**
>
> $$
> \begin{aligned}
> &= \hat{i}(1 - 6) \\
> &\quad - \hat{j}(2 + 12) \\
> &\quad + \hat{k}(-4 - 4)
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
**Problem**

Find the angle between vectors $\vec{a}$ and $\vec{b}$.

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
## 2. Systems of Equations

Find the values of $x$ and $y$ that satisfy both equations: $2x + 3y = 12$ and $x - y = 1$.
> **Solution:**
>
> From $x - y = 1$, we can write:
> $$x = y + 1$$
>
> Substituting this into the first equation:
> $$2(y + 1) + 3y = 12$$
> $$2y + 2 + 3y = 12$$
> $$5y = 10 \Rightarrow \mathbf{y = 2}$$
>
> Then finding $x$:
> $$x = 2 + 1 = \mathbf{3}$$

## 3. Proportionality

Consider the Universal Law of Gravitation: $F = G \frac{m_1 m_2}{r^2}$, where $F$ is the gravitational force between two masses $m_1$ and $m_2$, $r$ is the distance between their centers, and $G$ is the gravitational constant. Determine the factor by which the force $F$ changes if the distance $r$ is *doubled* and both masses ($m_1$ and $m_2$) are *halved*.
> **Solution:**
>
> Let the new force be $F'$:
> $$F' = G \frac{(\frac{1}{2}m_1)(\frac{1}{2}m_2)}{(2r)^2}$$
>
> $$F' = G \frac{\frac{1}{4}m_1 m_2}{4r^2} = \frac{1}{16} \left( G \frac{m_1 m_2}{r^2} \right)$$
>
> **Result:** The force $F$ decreases by a factor of **16**.

## 4. Rearranging Formulas

The formula for the period of a simple pendulum is $T = 2\pi \sqrt{\frac{L}{g}}$. Rearrange the equation give a formula for $g$ (acceleration due to gravity).
> **Solution:**
>
> 1. Divide both sides by $2\pi$:
> $$\frac{T}{2\pi} = \sqrt{\frac{L}{g}}$$
>
> 2. Square both sides to remove the square root:
> $$\frac{T^2}{4\pi^2} = \frac{L}{g}$$
>
> 3. Multiply by $g$ and divide by the left side to isolate $g$:
> $$\mathbf{g = \frac{4\pi^2 L}{T^2}}$$

## 5. Trigonometry

A vector $\vec{A}$ has a magnitude of $15$ and makes an angle of $\theta = 60^\circ$ with the horizontal axis. Calculate its horizontal and vertical components.
> **Solution:**
>
> Horizontal component ($A_x$):
> $$A_x = A \cdot \cos(\theta) = 15 \cdot \cos(60^\circ)$$
> $$A_x = 15 \cdot 0.5 = \mathbf{7.5}$$
>
> Vertical component ($A_y$):
> $$A_y = A \cdot \sin(\theta) = 15 \cdot \sin(60^\circ)$$
> $$A_y = 15 \cdot \frac{\sqrt{3}}{2} \approx \mathbf{12.99}$$

## 6. Function Analysis

Consider the function $f(x) = 3x^2 - 12x + 7$. Identify any local maxima or minima.
> **Solution:**
>
> 1. Find the first derivative and set it to zero:
> $$f'(x) = 6x - 12$$
> $$6x - 12 = 0 \Rightarrow \mathbf{x = 2}$$
>
> 2. Check the second derivative for the type of extremum:
> $$f''(x) = 6$$
> Since $f''(x) > 0$, the function has a **local minimum** at $x = 2$.
>
> 3. Find the $y$-value:
> $$f(2) = 3(2)^2 - 12(2) + 7 = 12 - 24 + 7 = \mathbf{-5}$$
> **Result:** Local minimum at $(2, -5)$.

## 7. Logic & Series

A bicycle is 10 meters from a wall and moves towards it at a constant speed of $1\text{ m/s}$. A fly starts from the bicycle's front wheel and flies towards the wall at $2\text{ m/s}$. When it hits the wall, it instantly turns back and flies to the bicycle, and so on. What is the total distance the fly travels before being crushed?
> **Solution:**
>
> Instead of summing an infinite series, we look at the total time:
> 1. Time for the bicycle to reach the wall:
> $$t = \frac{\text{distance}}{\text{speed}} = \frac{10\text{ m}}{1\text{ m/s}} = 10\text{ s}$$
>
> 2. The fly travels at a constant speed of $2\text{ m/s}$ during this entire 10 seconds:
> $$\text{Distance} = \text{speed} \cdot \text{time} = 2\text{ m/s} \cdot 10\text{ s} = \mathbf{20\text{ m}}$$
>
> Result: The fly travels 20 meters.
> This method avoids summing an infinite series.

## 8. Definite Integrals

Calculate the area under the curve of the function $f(x) = \sin(x)$ from $x=0$ to $x=\pi$.
> **Solution:**
>
> $$\text{Area} = \int_{0}^{\pi} \sin(x) \, dx$$
> $$\text{Area} = [-\cos(x)]_{0}^{\pi}$$
> $$\text{Area} = (-\cos(\pi)) - (-\cos(0))$$
> $$\text{Area} = (-(-1)) - (-1) = 1 + 1 = \mathbf{2}$$

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
