# Section 1: Mechanics I

## 1. Projectile Motion

A projectile is fired from the ground with an initial velocity of $100  \text{ m/s}$ at an angle of $37^\circ$ above the horizontal. Assume no air resistance.

> **Problem**
>
> Derive the equations of motion, time of flight, maximum height, and range.

> **Idea**
>
> Decompose the initial velocity into horizontal and vertical components. The horizontal motion is uniform (no acceleration), and the vertical motion is uniformly accelerated by gravity.
>
> $$
> v_{0x} = v_0 \cos\theta, \qquad v_{0y} = v_0 \sin\theta
> $$

---

* Derive the differential equations of motion in the horizontal and vertical directions.

> **Step 1 – Horizontal direction**
>
> No force acts horizontally, so:
>
> $$
> \ddot{x} = 0
> $$

> **Step 2 – Vertical direction**
>
> Gravity acts downward:
>
> $$
> \ddot{y} = -g
> $$

> **Result**
>
> $$
> \ddot{x} = 0, \qquad \ddot{y} = -g
> $$

---

* Determine the time of flight.

> **Step 1 – Integrate vertical equation**
>
> $$
> \dot{y}(t) = v_{0y} - gt = v_0\sin\theta - gt
> $$

> **Step 2 – Integrate again for position**
>
> $$
> y(t) = v_0\sin\theta \cdot t - \frac{1}{2}gt^2
> $$

> **Step 3 – Set $y = 0$ for landing**
>
> $$
> t\left(v_0\sin\theta - \frac{1}{2}gt\right) = 0
> $$

> **Step 4 – Take the non-zero solution**
>
> $$
> t_{\text{flight}} = \frac{2v_0\sin\theta}{g}
> $$

> **Step 5 – Substitute values** ($v_0 = 100$ m/s, $\theta = 37^\circ$, $g = 9.81$ m/s²)
>
> $$
> t_{\text{flight}} = \frac{2 \times 100 \times \sin 37^\circ}{9.81} = \frac{2 \times 100 \times 0.6018}{9.81} \approx 12.27 \text{ s}
> $$

> **Result**
>
> $$
> t_{\text{flight}} \approx 12.27 \text{ s}
> $$

---

* Determine the maximum height.

> **Step 1 – At maximum height, vertical velocity is zero**
>
> $$
> v_0\sin\theta - g t_{\text{top}} = 0 \implies t_{\text{top}} = \frac{v_0\sin\theta}{g}
> $$

> **Step 2 – Substitute into $y(t)$**
>
> $$
> H = v_0\sin\theta \cdot \frac{v_0\sin\theta}{g} - \frac{1}{2}g\left(\frac{v_0\sin\theta}{g}\right)^2
> $$

> **Step 3 – Simplify**
>
> $$
> H = \frac{v_0^2\sin^2\theta}{2g}
> $$

> **Step 4 – Substitute values**
>
> $$
> H = \frac{100^2 \times (0.6018)^2}{2 \times 9.81} \approx \frac{3622}{19.62} \approx 184.6 \text{ m}
> $$

> **Result**
>
> $$
> H \approx 184.6 \text{ m}
> $$

---

* Determine the range.

> **Step 1 – Horizontal position equation**
>
> $$
> x(t) = v_0\cos\theta \cdot t
> $$

> **Step 2 – Substitute $t_{\text{flight}}$**
>
> $$
> R = v_0\cos\theta \cdot \frac{2v_0\sin\theta}{g} = \frac{v_0^2 \sin(2\theta)}{g}
> $$

> **Step 3 – Substitute values** ($\sin 74^\circ \approx 0.9613$)
>
> $$
> R = \frac{100^2 \times 0.9613}{9.81} \approx 980 \text{ m}
> $$

> **Result**
>
> $$
> R \approx 980 \text{ m}
> $$

---

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

## 3. Path Intersection

Alice is moving along a path described by $A(t) = (2+t, 8-3t)$ and Bob is moving along a path $B(t) = (2t-1, 2t+2)$. Determine if their paths intersect. If yes, determine when and where they will collide. If not, determine the minimum distance between them and when it occurs.

> **Problem**
>
> Determine if the paths intersect, and if so, whether they collide (same place at the same time).

> **Idea**
>
> First check if the paths (curves in space) intersect by solving for $t_A$ and $t_B$ independently. Then check if $t_A = t_B$ for a collision.

> **Step 1 – Set x-coordinates equal**
>
> $$
> 2 + t_A = 2t_B - 1 \implies t_A = 2t_B - 3 \quad (1)
> $$

> **Step 2 – Set y-coordinates equal**
>
> $$
> 8 - 3t_A = 2t_B + 2 \implies 3t_A + 2t_B = 6 \quad (2)
> $$

> **Step 3 – Substitute (1) into (2)**
>
> $$
> 3(2t_B - 3) + 2t_B = 6
> $$
>
> $$
> 6t_B - 9 + 2t_B = 6 \implies 8t_B = 15 \implies t_B = \frac{15}{8}
> $$

> **Step 4 – Find $t_A$**
>
> $$
> t_A = 2 \times \frac{15}{8} - 3 = \frac{30}{8} - 3 = \frac{6}{8} = \frac{3}{4}
> $$

> **Step 5 – Find the intersection point**
>
> Using Alice's position at $t_A = \tfrac{3}{4}$:
>
> $$
> A\!\left(\tfrac{3}{4}\right) = \left(2 + \tfrac{3}{4},\ 8 - \tfrac{9}{4}\right) = \left(\tfrac{11}{4},\ \tfrac{23}{4}\right)
> $$

> **Step 6 – Check for collision**
>
> Since $t_A = \tfrac{3}{4} \neq t_B = \tfrac{15}{8}$, they are not at the same place at the same time.

> **Result**
>
> The **paths intersect** at the point $\left(\dfrac{11}{4},\ \dfrac{23}{4}\right)$, but Alice and Bob are **never there at the same time** — they do **not collide**.

---

## 4. Vector Calculus

The position of an object is given by $\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$. Find the object's velocity and acceleration vectors as a function of time.

> **Problem**
>
> Find the velocity and acceleration vectors as functions of time.

> **Idea**
>
> Velocity is the first derivative of position; acceleration is the second derivative.

> **Step 1 – Differentiate $\vec{r}(t)$ to get velocity**
>
> $$
> \vec{v}(t) = \frac{d\vec{r}}{dt} = 6t\,\hat{i} + (5 - 16t)\,\hat{j}
> $$

> **Step 2 – Differentiate $\vec{v}(t)$ to get acceleration**
>
> $$
> \vec{a}(t) = \frac{d\vec{v}}{dt} = 6\,\hat{i} - 16\,\hat{j}
> $$

> **Result**
>
> $$
> \vec{v}(t) = 6t\,\hat{i} + (5-16t)\,\hat{j}
> $$
>
> $$
> \vec{a}(t) = 6\,\hat{i} - 16\,\hat{j} \quad \text{(constant)}
> $$

---

## 5. Relative Velocity

A river flows east at $2 \text{m/s}$. A boat that can travel at $5 \text{m/s}$ in still water wants to go directly north across the river. In what direction (angle) should it head? How long will it take to cross the river if it's 200 meters wide?

> **Problem**
>
> Find the heading angle of the boat and the crossing time.

> **Idea**
>
> The boat must aim upstream (west of north) so that the river current cancels its westward component, resulting in a net northward velocity.

> **Step 1 – Set up the velocity components**
>
> Let $\phi$ be the angle west of north the boat heads. The net velocity must have zero eastward component:
>
> $$
> 5\sin\phi = 2
> $$

> **Step 2 – Solve for $\phi$**
>
> $$
> \sin\phi = \frac{2}{5} \implies \phi = \arcsin(0.4) \approx 23.6^\circ \text{ west of north}
> $$

> **Step 3 – Find the northward velocity component**
>
> $$
> v_N = 5\cos\phi = 5\sqrt{1 - 0.16} = 5\sqrt{0.84} \approx 4.58 \text{ m/s}
> $$

> **Step 4 – Compute crossing time**
>
> $$
> t = \frac{200}{v_N} = \frac{200}{4.58} \approx 43.7 \text{ s}
> $$

> **Result**
>
> The boat should head $\approx 23.6^\circ$ **west of north**.
>
> Crossing time $\approx 43.7$ s.

---

## 6. Variable Velocity

An object's velocity is given by $v(t) = t^2 + 2t - 5$. If the object was at $x=4$ at $t=0$, what is its position and acceleration at time $t=3$?

## 7. Elimination of time and interpretation of acceleration

The path equation is given in parametric form:

$$
x(t)=2t^2, \qquad y(t)=3t^3
$$

* Eliminate the parameter $t$.
* Draw the trajectory.
* Calculate $\vec v(t)$, $|\vec v(t)|$, $\vec a(t)$ and $|\vec a(t)|$.
* Is the acceleration constant?


## 8. Circular Motion

Calculate the centripetal acceleration of a person standing on the Earth's equator. The Earth's radius is approximately 6378 km.

## 9. Momentum Comparison

Which has greater momentum: a 2-gram fly flying at $10$ m/s or a 60-gram tennis ball moving at $1$ m/s?


## 10. Kinematics

Point M moves according to the equation:

$$
\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)
$$

where $a, b, \omega$ are positive constants.

a) Find the equation of the point's trajectory,

b) Compute the path length of the point from time $t=0$ to $t=t_0$,

c) Draw the trajectory of this point using Python or interactive HTML. Discuss special cases.
