## 2. Range Optimization

For projectile motion, show analytically that the maximum range $R(\theta)=\frac{v_0^2 \sin(2\theta)}{g}
$ for a given initial velocity is achieved at a launch angle of $45^\circ$.

> **Problem**
>
> Find the angle $\theta$ that maximizes $R(\theta)$.

> **Idea**
>
> Differentiate $R(\theta)$ with respect to $\theta$, set the derivative to zero, and solve.

> **Step 1 – Write the range function**
>
> $$
> R(\theta) = \frac{v_0^2}{g}\sin(2\theta)
> $$

> **Step 2 – Differentiate with respect to $\theta$**
>
> $$
> \frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta)
> $$

> **Step 3 – Set equal to zero**
>
> $$
> 2\cos(2\theta) = 0 \implies \cos(2\theta) = 0
> $$

> **Step 4 – Solve**
>
> $$
> 2\theta = 90^\circ \implies \theta = 45^\circ
> $$

> **Step 5 – Verify it is a maximum**
>
> $$
> \frac{d^2R}{d\theta^2} = -\frac{4v_0^2}{g}\sin(2\theta)\bigg|_{\theta=45^\circ} = -\frac{4v_0^2}{g} < 0 \quad \checkmark
> $$

> **Result**
>
> The range is maximized at $\theta = 45^\circ$, giving:
>
> $$
> R_{\max} = \frac{v_0^2}{g}
> $$

---
