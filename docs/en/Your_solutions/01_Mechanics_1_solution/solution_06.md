## 6. Variable Velocity

An object's velocity is given by $v(t) = t^2 + 2t - 5$. If the object was at $x=4$ at $t=0$, what is its position and acceleration at time $t=3$?

> **Problem**
>
> Determine the position $x(3)$ and the acceleration $a(3)$.

> **Idea**
>
> Position is obtained by integrating the velocity function ($v = dx/dt$) and using the initial condition to find the constant of integration. Acceleration is obtained by differentiating the velocity function ($a = dv/dt$).

---

* Determine the position at $t=3$.

> **Step 1 – Integrate velocity to find the general position function**
>
> $$
> v(t) = \frac{dx}{dt} = t^2 + 2t - 5
> $$
>
> $$
> x(t) = \int (t^2 + 2t - 5)\,dt = \frac{t^3}{3} + t^2 - 5t + C
> $$

> **Step 2 – Apply the initial condition $x(0) = 4$**
>
> $$
> x(0) = \frac{0^3}{3} + 0^2 - 5(0) + C = 4 \implies C = 4
> $$
>
> $$
> x(t) = \frac{t^3}{3} + t^2 - 5t + 4
> $$

> **Step 3 – Evaluate position at $t = 3$**
>
> $$
> x(3) = \frac{3^3}{3} + 3^2 - 5(3) + 4
> $$
>
> $$
> x(3) = \frac{27}{3} + 9 - 15 + 4 = 9 + 9 - 15 + 4 = 7
> $$

> **Result**
>
> $$
> x(3) = 7 \text{ m}
> $$

---

* Determine the acceleration at $t=3$.

> **Step 1 – Differentiate velocity to find acceleration**
>
> $$
> a(t) = \frac{dv}{dt} = \frac{d}{dt}(t^2 + 2t - 5)
> $$
>
> $$
> a(t) = 2t + 2
> $$

> **Step 2 – Evaluate acceleration at $t = 3$**
>
> $$
> a(3) = 2(3) + 2 = 6 + 2 = 8
> $$

> **Result**
>
> $$
> a(3) = 8 \text{ m/s}^2
> $$
>
> <div align="center">
>  <img src="velocity_acceleration_plots.png" width="600" alt="Velocity and Acceleration Plots">
> </div>

---
