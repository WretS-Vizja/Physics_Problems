# 3. Superposition Principle

## Problem
Two waves are described by the equations $y_1(x, t) = A \sin(kx - \omega t)$ and $y_2(x, t) = A \sin(kx + \omega t)$. What is the equation of the resulting standing wave? Identify the positions of the nodes.

## Solution

**Step 1 — Apply the superposition principle.**  
The total displacement is the sum of the two waves:

$$y(x,t) = y_1 + y_2 = A\sin(kx-\omega t) + A\sin(kx+\omega t)$$

**Step 2 — Use the sum-to-product identity.**  

$$\sin\alpha + \sin\beta = 2\sin\!\left(\frac{\alpha+\beta}{2}\right)\cos\!\left(\frac{\alpha-\beta}{2}\right)$$

With $\alpha = kx-\omega t$ and $\beta = kx+\omega t$:

- $\dfrac{\alpha+\beta}{2} = kx$  
- $\dfrac{\alpha-\beta}{2} = -\omega t$, and $\cos(-\omega t) = \cos(\omega t)$

**Step 3 — Write the resulting standing wave.**  

$$y(x,t) = 2A\sin(kx)\cos(\omega t)$$

The spatial part $\sin(kx)$ and the temporal part $\cos(\omega t)$ are **separated**, which is the signature of a standing wave: every point oscillates in time with an amplitude that depends only on $x$.

**Step 4 — Locate the nodes.**  
A node is a point with zero displacement at all times. This requires

$$\sin(kx_n) = 0 \quad\Longrightarrow\quad kx_n = n\pi,\quad n = 0, 1, 2, \ldots$$

Substituting $k = 2\pi/\lambda$:

$$x_n = \frac{n\pi}{k} = \frac{n\lambda}{2}$$

**Step 5 — Locate the antinodes (for context).**  
Antinodes (maximum amplitude) occur where $|\sin(kx)| = 1$:

$$x_m = (2m+1)\frac{\lambda}{4},\quad m = 0, 1, 2, \ldots$$

## Answer

$$\boxed{y(x,t) = 2A\sin(kx)\cos(\omega t),\qquad x_n = \frac{n\lambda}{2}\ (n = 0,1,2,\ldots)}$$
