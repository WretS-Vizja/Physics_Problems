# 10. Force field and power

In a certain force field, the equations of motion of a particle with mass $m=0.5$ kg are as follows:

$$
x = 5t^2 - t, \quad y = 2t^3, \quad z = -3t + 2
$$

Find the time dependence of: the particle's velocity, the particle's momentum, the particle's acceleration, the force acting on the particle, and the power transferred by the field to the particle.

> **Idea**
>
> We are given position as a function of time. All other quantities follow by successive differentiation and multiplication:
>
> $$\vec{r}(t) \xrightarrow{d/dt} \vec{v}(t) \xrightarrow{d/dt} \vec{a}(t) \xrightarrow{\times m} \vec{F}(t)$$
>
> Momentum is $\vec{p} = m\vec{v}$, and power is $P = \vec{F} \cdot \vec{v}$.

## (a) Velocity: $\vec{v}(t) = \dot{\vec{r}}(t)$

> **Step 1 – Differentiate each position component**
>
> $$v_x = \frac{dx}{dt} = \frac{d}{dt}(5t^2 - t) = 10t - 1$$
>
> $$v_y = \frac{dy}{dt} = \frac{d}{dt}(2t^3) = 6t^2$$
>
> $$v_z = \frac{dz}{dt} = \frac{d}{dt}(-3t + 2) = -3$$
>
> $$\boxed{\vec{v}(t) = (10t - 1,\ 6t^2,\ -3) \text{ m/s}}$$
>
> **Note:** At $t = 0$, the velocity is $(-1, 0, -3)$ m/s. The $v_x$ component changes sign at $t = 0.1$ s. The $z$-component is constant — no acceleration in $z$.

## (b) Momentum: $\vec{p}(t) = m\vec{v}(t)$

> **Step 2 – Multiply velocity by mass**
>
> $$\vec{p}(t) = 0.5 \times (10t - 1,\ 6t^2,\ -3)$$
>
> $$\boxed{\vec{p}(t) = (5t - 0.5,\ 3t^2,\ -1.5) \text{ kg·m/s}}$$
>
> **Note:** The $z$-momentum is constant at $-1.5$ kg·m/s, confirming $F_z = dp_z/dt = 0$.

## (c) Acceleration: $\vec{a}(t) = \dot{\vec{v}}(t)$

> **Step 3 – Differentiate each velocity component**
>
> $$a_x = \frac{dv_x}{dt} = \frac{d}{dt}(10t - 1) = 10$$
>
> $$a_y = \frac{dv_y}{dt} = \frac{d}{dt}(6t^2) = 12t$$
>
> $$a_z = \frac{dv_z}{dt} = \frac{d}{dt}(-3) = 0$$
>
> $$\boxed{\vec{a}(t) = (10,\ 12t,\ 0) \text{ m/s}^2}$$
>
> **Physical interpretation:** Constant acceleration in $x$ (steady force), linearly growing acceleration in $y$ (increasing force), and zero acceleration in $z$ (free motion).

## (d) Force: $\vec{F}(t) = m\vec{a}(t)$

> **Step 4 – Multiply acceleration by mass**
>
> $$\vec{F}(t) = 0.5 \times (10,\ 12t,\ 0)$$
>
> $$\boxed{\vec{F}(t) = (5,\ 6t,\ 0) \text{ N}}$$
>
> **Verification via $\vec{F} = d\vec{p}/dt$:** $F_x = \frac{d}{dt}(5t - 0.5) = 5$ ✓, $F_y = \frac{d}{dt}(3t^2) = 6t$ ✓, $F_z = \frac{d}{dt}(-1.5) = 0$ ✓

## (e) Power: $P(t) = \vec{F} \cdot \vec{v}$

> **Step 5 – Compute the dot product**
>
> Power is the rate at which the force transfers energy to the particle:
>
> $$P(t) = F_x v_x + F_y v_y + F_z v_z$$
>
> $$P(t) = 5 \cdot (10t - 1) + 6t \cdot 6t^2 + 0 \cdot (-3)$$
>
> $$P(t) = (50t - 5) + 36t^3 + 0$$
>
> $$\boxed{P(t) = 36t^3 + 50t - 5 \text{ W}}$$
>
> **Note:** At $t = 0$, $P(0) = -5$ W (the force is doing negative work, decelerating the particle). For large $t$, the $36t^3$ term dominates.
>
> **Verification with KE:** $KE = \frac{1}{2}(0.5)[(10t-1)^2 + (6t^2)^2 + 9]$. Taking $dKE/dt$:
>
> $$\frac{dKE}{dt} = \frac{1}{4}[2(10t-1)(10) + 2(6t^2)(12t)] = 5(10t-1) + 36t^3 = 50t - 5 + 36t^3 \quad \checkmark$$
