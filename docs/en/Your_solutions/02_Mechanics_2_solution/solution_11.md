# 11. Dynamics with a time-dependent force

A particle of mass $m=3$ kg moves in a force field $F$ dependent on time in the following way:

$$
F = (15t, 3t-12, -6t^2) \, \text{N}
$$

Assuming initial conditions $r_0=(5,2,-3)$ m, $v_0=(2,0,1)$ m/s, find the dependence of the particle's position and velocity on time.

> **Idea**
>
> This is the reverse of Problem 10: instead of differentiating position to get force, we start with force and integrate to get velocity and position:
>
> $$\vec{F}(t) \xrightarrow{\div m} \vec{a}(t) \xrightarrow{\int dt} \vec{v}(t) \xrightarrow{\int dt} \vec{r}(t)$$
>
> Each integration introduces a constant determined by the initial conditions.

## (a) Acceleration

> **Step 1 – Find the acceleration from Newton's 2nd law**
>
> $$\vec{a}(t) = \frac{\vec{F}(t)}{m} = \left(\frac{15t}{3},\ \frac{3t-12}{3},\ \frac{-6t^2}{3}\right) = (5t,\ t - 4,\ -2t^2) \text{ m/s}^2$$
>
> **Observations:** The $x$-acceleration grows linearly; the $y$-acceleration starts at $-4$ m/s² and crosses zero at $t = 4$ s; the $z$-acceleration is always negative and grows in magnitude.

## (b) Velocity: $\vec{v}(t) = \vec{v}_0 + \int_0^t \vec{a}(\tau)\,d\tau$

> **Step 2 – Integrate the x-component**
>
> $$v_x(t) = 2 + \int_0^t 5\tau\,d\tau = 2 + \left[\frac{5\tau^2}{2}\right]_0^t = 2 + \frac{5t^2}{2}$$
>
> Starts at 2 m/s and always increases.

> **Step 3 – Integrate the y-component**
>
> $$v_y(t) = 0 + \int_0^t (\tau - 4)\,d\tau = \left[\frac{\tau^2}{2} - 4\tau\right]_0^t = \frac{t^2}{2} - 4t$$
>
> Initially negative ($v_y < 0$ for $0 < t < 8$ s), reverses direction at $t = 8$ s.

> **Step 4 – Integrate the z-component**
>
> $$v_z(t) = 1 + \int_0^t (-2\tau^2)\,d\tau = 1 + \left[-\frac{2\tau^3}{3}\right]_0^t = 1 - \frac{2t^3}{3}$$
>
> Starts at 1 m/s and decreases rapidly due to the $t^3$ term.

> **Result**
>
> $$\boxed{\vec{v}(t) = \left(2 + \frac{5t^2}{2},\ \ \frac{t^2}{2} - 4t,\ \ 1 - \frac{2t^3}{3}\right) \text{ m/s}}$$

## (c) Position: $\vec{r}(t) = \vec{r}_0 + \int_0^t \vec{v}(\tau)\,d\tau$

> **Step 5 – Integrate the x-component**
>
> $$x(t) = 5 + \int_0^t \left(2 + \frac{5\tau^2}{2}\right)d\tau = 5 + \left[2\tau + \frac{5\tau^3}{6}\right]_0^t = 5 + 2t + \frac{5t^3}{6}$$

> **Step 6 – Integrate the y-component**
>
> $$y(t) = 2 + \int_0^t \left(\frac{\tau^2}{2} - 4\tau\right)d\tau = 2 + \left[\frac{\tau^3}{6} - 2\tau^2\right]_0^t = 2 + \frac{t^3}{6} - 2t^2$$

> **Step 7 – Integrate the z-component**
>
> $$z(t) = -3 + \int_0^t \left(1 - \frac{2\tau^3}{3}\right)d\tau = -3 + \left[\tau - \frac{\tau^4}{6}\right]_0^t = -3 + t - \frac{t^4}{6}$$

> **Result**
>
> $$\boxed{\vec{r}(t) = \left(5 + 2t + \frac{5t^3}{6},\ \ 2 + \frac{t^3}{6} - 2t^2,\ \ -3 + t - \frac{t^4}{6}\right) \text{ m}}$$
>
> **Verification at $t = 0$:** $\vec{r}(0) = (5, 2, -3)$ ✓
