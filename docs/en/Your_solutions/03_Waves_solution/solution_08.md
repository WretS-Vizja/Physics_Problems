# 8. Waves

## Problem
Which of the following functions can describe a traveling wave? Hint: check if it satisfies the wave equation

$$\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}$$

a) $y(x,t) = A \cos(kx^2 - \omega t)$  
b) $y(x,t) = A(x-vt)^2$  
c) $y(x,t) = A \log(x+vt)$

## Solution

**General principle.**  
Any function of the form $f(x \pm vt)$ automatically satisfies the 1-D wave equation. So the quickest check is: can the argument be written as a pure combination $x \pm vt$? If yes, it is a wave. If not, we must compute the partial derivatives explicitly.

### a) $y = A\cos(kx^2 - \omega t)$

The argument $kx^2 - \omega t$ is **not** of the form $x \pm vt$ because of the $x^2$. Verify by explicit differentiation.

**$x$-derivatives:**

$$\frac{\partial y}{\partial x} = -A\sin(kx^2 - \omega t)\cdot 2kx$$

$$\frac{\partial^2 y}{\partial x^2} = -4k^2 x^2\,A\cos(kx^2-\omega t) - 2kA\sin(kx^2-\omega t)$$

**$t$-derivatives:**

$$\frac{\partial^2 y}{\partial t^2} = -\omega^2 A\cos(kx^2-\omega t)$$

For the wave equation to hold, we would need

$$-4k^2 x^2 A\cos(\cdot) - 2kA\sin(\cdot) = -\frac{\omega^2}{v^2}A\cos(\cdot)$$

The right-hand side has **no sine term** and **no explicit $x$-dependence** in its coefficient, while the left-hand side has both. Equality cannot hold for every $x$ and $t$.

**→ Not a traveling wave.** ❌

### b) $y = A(x - vt)^2$

The argument is already in $f(x - vt)$ form, so it must be a wave. Let's verify.

**$x$-derivatives:**

$$\frac{\partial y}{\partial x} = 2A(x-vt),\qquad \frac{\partial^2 y}{\partial x^2} = 2A$$

**$t$-derivatives:**

$$\frac{\partial y}{\partial t} = -2Av(x-vt),\qquad \frac{\partial^2 y}{\partial t^2} = 2Av^2$$

**Check:**

$$\frac{1}{v^2}\cdot 2Av^2 = 2A \;=\; \frac{\partial^2 y}{\partial x^2}\quad\checkmark$$

**→ Traveling wave.** ✅  
(Mathematically valid, though physically unrealistic because the amplitude grows without bound.)

### c) $y = A\log(x + vt)$

The argument is of the form $f(x + vt)$, so it represents a wave moving in the $-x$ direction. Verify.

**$x$-derivatives:**

$$\frac{\partial y}{\partial x} = \frac{A}{x+vt},\qquad \frac{\partial^2 y}{\partial x^2} = -\frac{A}{(x+vt)^2}$$

**$t$-derivatives:**

$$\frac{\partial y}{\partial t} = \frac{Av}{x+vt},\qquad \frac{\partial^2 y}{\partial t^2} = -\frac{Av^2}{(x+vt)^2}$$

**Check:**

$$\frac{1}{v^2}\cdot\left(-\frac{Av^2}{(x+vt)^2}\right) = -\frac{A}{(x+vt)^2} \;=\; \frac{\partial^2 y}{\partial x^2}\quad\checkmark$$

**→ Traveling wave.** ✅

## Answer

| Function | Traveling wave? |
|---|---|
| a) $A\cos(kx^2 - \omega t)$ | **No** |
| b) $A(x - vt)^2$ | **Yes** (propagates in $+x$ direction) |
| c) $A\log(x + vt)$ | **Yes** (propagates in $-x$ direction) |
