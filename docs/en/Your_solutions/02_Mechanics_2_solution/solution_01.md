## 1. Gravitational Dependence
 
A simple pendulum has a period of 4 seconds on Earth. What would its period be on the Moon, where the gravitational acceleration is about 1/6th of Earth's?
 
What is the required length of a simple pendulum to have a period of exactly 1 second on Earth?
 
### Part A — Period on the Moon
 
> **Problem**
>
> A simple pendulum with period $T_E = 4$ s on Earth is taken to the Moon where $g_M = g_E / 6$. Find the new period $T_M$.
 
> **Idea**
>
> The period of a simple pendulum is given by $T = 2\pi\sqrt{L/g}$. Notice that $T$ depends on two things: the length $L$ of the string and the local gravitational acceleration $g$. Crucially, $T$ does **not** depend on the mass of the bob. Since we are taking the same pendulum (same $L$) to the Moon, only $g$ changes. Because $g$ appears in the denominator under the square root, a smaller $g$ leads to a longer period — the pendulum swings more slowly on the Moon.
 
> **Step 1 – Write the period formulas**
>
> On Earth, the period is:
>
> $$T_E = 2\pi\sqrt{\frac{L}{g_E}}$$
>
> On the Moon, the same pendulum has:
>
> $$T_M = 2\pi\sqrt{\frac{L}{g_M}}$$
>
> Here $g_E \approx 9.81$ m/s² and $g_M \approx g_E/6 \approx 1.635$ m/s². The length $L$ is identical in both equations since we are physically transporting the same pendulum.
 
> **Step 2 – Take the ratio to eliminate $L$**
>
> Dividing the Moon expression by the Earth expression, $2\pi$ and $\sqrt{L}$ cancel:
>
> $$\frac{T_M}{T_E} = \frac{2\pi\sqrt{L/g_M}}{2\pi\sqrt{L/g_E}} = \sqrt{\frac{g_E}{g_M}}$$
>
> This is a powerful technique: by taking a ratio, we avoid needing to know the actual length of the pendulum.
 
> **Step 3 – Substitute $g_M = g_E/6$**
>
> $$\frac{T_M}{T_E} = \sqrt{\frac{g_E}{g_E/6}} = \sqrt{6}$$
>
> The factor of $g_E$ cancels completely, leaving only the ratio 6 inside the square root. This tells us that the Moon period is $\sqrt{6}$ times longer than the Earth period, regardless of what $g_E$ actually is.
 
> **Step 4 – Solve**
>
> $$T_M = T_E \cdot \sqrt{6} = 4 \cdot \sqrt{6} \approx 4 \times 2.449 = 9.80 \text{ s}$$
>
> **Physical check:** The period increased from 4 s to ~9.8 s — roughly 2.45 times longer. This makes sense: weaker gravity means a weaker restoring force, so the pendulum takes longer to complete each swing.
 
> **Result**
>
> $$\boxed{T_M \approx 9.80 \text{ s}}$$
 
---
 
### Part B — Required Length for $T = 1$ s
 
> **Problem**
>
> Find the length $L$ such that the pendulum period is exactly 1 s on Earth.
 
> **Idea**
>
> We need to invert the period formula to solve for $L$. Since $T = 2\pi\sqrt{L/g}$, we can square both sides and isolate $L$.
 
> **Step 1 – Solve the period formula for $L$**
>
> Starting from:
>
> $$T = 2\pi\sqrt{\frac{L}{g}}$$
>
> Square both sides to remove the square root:
>
> $$T^2 = 4\pi^2 \frac{L}{g}$$
>
> Multiply both sides by $g$ and divide by $4\pi^2$:
>
> $$L = \frac{gT^2}{4\pi^2}$$
 
> **Step 2 – Substitute values**
>
> With $g = 9.81$ m/s² and $T = 1$ s:
>
> $$L = \frac{9.81 \times 1^2}{4\pi^2} = \frac{9.81}{4 \times 9.8696} = \frac{9.81}{39.478}$$
>
> Note: $\pi^2 \approx 9.8696$, so $4\pi^2 \approx 39.478$.
 
> **Step 3 – Calculate**
>
> $$L = 0.2485 \text{ m} \approx 0.249 \text{ m}$$
>
> **Unit check:** $\frac{[\text{m/s}^2][\text{s}^2]}{[\text{dimensionless}]} = \text{m}$ ✓
>
> **Physical check:** A quarter-meter pendulum having a 1-second period is consistent with everyday experience — grandfather clocks use pendulums of about 1 meter for a 2-second period, so halving the period to 1 s requires roughly $1/4$ the length (since $T \propto \sqrt{L}$, halving $T$ means quartering $L$).
 
> **Result**
>
> $$\boxed{L \approx 0.249 \text{ m} \approx 24.9 \text{ cm}}$$
 
---
