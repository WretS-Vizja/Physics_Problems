# Section 0: Mathematical Foundations

## 1. Vector Algebra

Given two vectors in 3D space: $\vec{a} = [2, 1, -3]$ and $\vec{b} = [4, -2, 1]$. Calculate:

a) The magnitude of each vector.
> **Solution:**
>
> Using the magnitude formula:
> $$|\vec{v}| = \sqrt{v_x^2 + v_y^2 + v_z^2}$$
>
> For vector $\vec{a}$:
> $$|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2} = \sqrt{4 + 1 + 9} = \mathbf{\sqrt{14}}$$
>
> For vector $\vec{b}$:
> $$|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2} = \sqrt{16 + 4 + 1} = \mathbf{\sqrt{21}}$$

b) The dot product $\vec{a} \cdot \vec{b}$.
> **Solution:**
>
> $$\vec{a} \cdot \vec{b} = (a_x \cdot b_x) + (a_y \cdot b_y) + (a_z \cdot b_z)$$
> $$\vec{a} \cdot \vec{b} = (2 \cdot 4) + (1 \cdot -2) + (-3 \cdot 1)$$
> $$\vec{a} \cdot \vec{b} = 8 - 2 - 3 = \mathbf{3}$$

c) The cross product $\vec{a} \times \vec{b}$.
> **Solution:**
>
> $$\vec{a} \times \vec{b} = \begin{vmatrix} \mathbf{\hat{i}} & \mathbf{\hat{j}} & \mathbf{\hat{k}} \\ 2 & 1 & -3 \\ 4 & -2 & 1 \end{vmatrix}$$
>
> $$= \mathbf{\hat{i}}[(1)(1) - (-3)(-2)] - \mathbf{\hat{j}}[(2)(1) - (-3)(4)] + \mathbf{\hat{k}}[(2)(-2) - (1)(4)]$$
> $$= \mathbf{\hat{i}}(1 - 6) - \mathbf{\hat{j}}(2 + 12) + \mathbf{\hat{k}}(-4 - 4)$$
> $$= \mathbf{[-5, -14, -8]}$$

d) The angle between vectors $\vec{a}$ and $\vec{b}$.
> **Solution:**
>
> $$\cos\theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}||\vec{b}|}$$
>
> $$\cos\theta = \frac{3}{\sqrt{14}\sqrt{21}} = \frac{3}{\sqrt{294}}$$
>
> $$\theta = \arccos\left(\frac{3}{\sqrt{294}}\right) \approx \mathbf{79.9^\circ}$$

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

## 5. Trigonometry

A vector $\vec{A}$ has a magnitude of $15$ and makes an angle of $\theta = 60^\circ$ with the horizontal axis. Calculate its horizontal and vertical components.

## 6. Function Analysis

Consider the function $f(x) = 3x^2 - 12x + 7$. Identify any local maxima or minima.

## 7. Logic & Series

A bicycle is 10 meters from a wall and moves towards it at a constant speed of $1\text{ m/s}$. A fly starts from the bicycle's front wheel and flies towards the wall at $2\text{ m/s}$. When it hits the wall, it instantly turns back and flies to the bicycle, and so on. What is the total distance the fly travels before being crushed?

## 8. Definite Integrals

Calculate the area under the curve of the function $f(x) = \sin(x)$ from $x=0$ to $x=\pi$.

## 9. Optimization Problem

A rectangle is under the curve $y = 3 - x^2$ in the first quadrant. What are the dimensions of the rectangle with the maximum area?

## 10. Infinite Series

Determine the final position of an ant that starts at the origin and moves according to the following pattern: 1 m east, 1/2 m north, 1/3 m west, 1/4 m south, 1/5 m east, and so on.
