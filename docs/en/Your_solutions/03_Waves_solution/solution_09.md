# 9. Damped oscillator

## Problem
For the given equation describing a damped harmonic oscillator:

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = 0
$$

make interactive HTML animation with a slider for the parameter $b$ to show the behavior of the system in the underdamped, critically damped, and overdamped cases. Include graphs of $x(t)$ and the phase portrait for each case.

1. Write down the general solution.
2. Present the classification of cases: underdamped, critically damped, overdamped.
3. Solve the equation numerically (RK4).
4. Investigate the effect of parameter $b$.
5. Generate the graph of $x(t)$.
6. Generate the phase portrait.

## Solution

### 1. General solution

**Step 1 — Substitute the trial solution $x(t) = e^{rt}$.**  
Substituting into $m\ddot{x} + b\dot{x} + kx = 0$ gives the **characteristic equation**

$$mr^2 + br + k = 0$$

**Step 2 — Solve for $r$.**  

$$r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}$$

**Step 3 — Introduce standard parameters.**  
Define the damping coefficient and natural frequency:

$$\gamma \equiv \frac{b}{2m},\qquad \omega_0 \equiv \sqrt{\frac{k}{m}}$$

Then

$$r_{1,2} = -\gamma \pm \sqrt{\gamma^2 - \omega_0^2}$$

The sign of the discriminant $\Delta = b^2 - 4mk = 4m^2(\gamma^2 - \omega_0^2)$ determines the behavior.

### 2. Classification of the three cases

**Underdamped** ($b < 2\sqrt{mk}$, i.e. $\gamma < \omega_0$):  
Roots are complex conjugates. The motion oscillates with exponentially decaying amplitude:

$$x(t) = e^{-\gamma t}\bigl[C_1\cos(\omega_d t) + C_2\sin(\omega_d t)\bigr],\qquad \omega_d = \sqrt{\omega_0^2 - \gamma^2}$$

**Critically damped** ($b = 2\sqrt{mk}$, i.e. $\gamma = \omega_0$):  
Repeated real root $r = -\gamma$. The system returns to equilibrium as fast as possible without oscillating:

$$x(t) = (C_1 + C_2\, t)\, e^{-\gamma t}$$

**Overdamped** ($b > 2\sqrt{mk}$, i.e. $\gamma > \omega_0$):  
Two distinct real negative roots. The system decays exponentially without oscillation, slower than in the critical case:

$$x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t},\qquad r_{1,2} = -\gamma \pm \sqrt{\gamma^2 - \omega_0^2}$$

### 3. Numerical solution (RK4)

**Step 1 — Convert to a first-order system.**  
Let $v = \dot{x}$. The second-order ODE becomes two coupled first-order equations:

$$\dot{x} = v,\qquad \dot{v} = -\frac{b}{m}v - \frac{k}{m}x$$

**Step 2 — RK4 step.**  
Writing the state as $\mathbf{y} = (x, v)$ and the right-hand side as $\mathbf{f}(\mathbf{y})$:

$$
\begin{aligned}
\mathbf{k}_1 &= \mathbf{f}(\mathbf{y}_n) \\
\mathbf{k}_2 &= \mathbf{f}(\mathbf{y}_n + \tfrac{h}{2}\mathbf{k}_1) \\
\mathbf{k}_3 &= \mathbf{f}(\mathbf{y}_n + \tfrac{h}{2}\mathbf{k}_2) \\
\mathbf{k}_4 &= \mathbf{f}(\mathbf{y}_n + h\,\mathbf{k}_3) \\
\mathbf{y}_{n+1} &= \mathbf{y}_n + \frac{h}{6}(\mathbf{k}_1 + 2\mathbf{k}_2 + 2\mathbf{k}_3 + \mathbf{k}_4)
\end{aligned}
$$

Implementation in JavaScript (used in the HTML animation):

```javascript
function deriv(x, v) {
  return { dx: v, dv: -(b/m)*v - (k/m)*x };
}
function rk4(x, v, dt) {
  const k1 = deriv(x, v);
  const k2 = deriv(x + k1.dx*dt/2, v + k1.dv*dt/2);
  const k3 = deriv(x + k2.dx*dt/2, v + k2.dv*dt/2);
  const k4 = deriv(x + k3.dx*dt,   v + k3.dv*dt);
  return {
    x: x + dt/6*(k1.dx + 2*k2.dx + 2*k3.dx + k4.dx),
    v: v + dt/6*(k1.dv + 2*k2.dv + 2*k3.dv + k4.dv)
  };
}
```

### 4. Effect of the parameter $b$

Increasing $b$ (more damping) has the following qualitative effects:

- The **envelope** $e^{-\gamma t}$ decays faster, because $\gamma = b/(2m)$ grows linearly with $b$.  
- The **oscillation frequency** $\omega_d = \sqrt{\omega_0^2 - \gamma^2}$ decreases; when $b$ reaches $2\sqrt{mk}$, $\omega_d = 0$ and oscillations disappear entirely.  
- For $b > 2\sqrt{mk}$ there is no oscillation at all; the return to equilibrium becomes progressively slower as $b$ grows (overdamped regime).  
- The minimum return time to equilibrium is achieved at **critical damping** $b = 2\sqrt{mk}$.

### 5 & 6. Graphs of $x(t)$ and the phase portrait

- The $x(t)$ plot shows damped oscillations (underdamped), a smooth monotone return (critical), or a slower monotone return (overdamped).  
- The phase portrait $(x, \dot{x})$ shows an **inward spiral** for underdamped motion and a **direct sweep toward the origin** (node) for critical/overdamped cases.

### Interactive animation

📄 **[09_damped_oscillator.html](./09_damped_oscillator.html)** — Sliders for $m$, $k$, $b$, initial conditions, and preset buttons for each regime. Plots $x(t)$ and the phase portrait side-by-side in real time.

## Answer

$$
\boxed{
\begin{array}{ll}
\text{Underdamped } (b<2\sqrt{mk}): & x(t) = e^{-\gamma t}[C_1\cos\omega_d t + C_2\sin\omega_d t] \\
\text{Critical } (b=2\sqrt{mk}): & x(t) = (C_1 + C_2 t)\,e^{-\gamma t} \\
\text{Overdamped } (b>2\sqrt{mk}): & x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t}
\end{array}
}
$$
