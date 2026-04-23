# 10. Animation: Wave Sources

## Problem
Write an HTML animation in which it is possible to place dots that will serve as sources of waves described by the equation:

$$
u(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_0}|^\alpha} \sin(k |\vec{r} - \vec{r_0}| - \omega t)
$$

where $\vec{r_0}$ is the position of the dot, and $\alpha$ is a parameter that can be set within the range $[0, 2]$. The animation should show the superposition of waves from all dots.

## Solution

### Physical idea

Each source placed at $\vec{r}_i$ radiates an outgoing circular wave whose amplitude falls off with distance as $1/r^\alpha$. The total displacement at any point $\vec{r}$ at time $t$ is the sum over all sources:

$$u_{\text{total}}(\vec{r}, t) = \sum_{i} \frac{A}{|\vec{r}-\vec{r}_i|^\alpha}\, \sin\bigl(k|\vec{r}-\vec{r}_i| - \omega t\bigr)$$

### Role of $\alpha$

| $\alpha$ | Physical interpretation | Amplitude behavior |
|---|---|---|
| 0 | No geometric attenuation (like a plane wave) | Constant with distance |
| 0.5 | 2-D cylindrical wave (energy conservation) | $\propto 1/\sqrt{r}$ |
| 1 | "Strong" cylindrical attenuation | $\propto 1/r$ |
| 2 | 3-D spherical wave (energy conservation in 3D) | $\propto 1/r^2$ |

### Implementation steps

**Step 1 — Collect sources.** Use an array `sources = []`. On each canvas click, push `{x, y}`.

**Step 2 — Sample the wave field.** At every frame and every pixel (or every $4\times 4$ block for performance), compute

```javascript
let u = 0;
for (const s of sources) {
  const r = Math.hypot(px - s.x, py - s.y) + 1;  // +1 avoids division by zero
  u += A / Math.pow(r, alpha) * Math.sin(k*r - omega*t);
}
```

**Step 3 — Map $u$ to color.** Normalize and use a red-blue diverging colormap: positive crests → red, troughs → blue.

**Step 4 — Advance time.** Increment $t$ each animation frame; redraw using `requestAnimationFrame`.

### Interactive animation

📄 **[10_wave_sources.html](./10_wave_sources.html)** — Click anywhere on the canvas to add a source. Sliders control $\alpha$, $\lambda$, and $\omega$. Preset buttons add two or four sources arranged symmetrically.

### Things to observe

- **One source:** outgoing concentric circles.  
- **Two sources:** classic two-source interference pattern (hyperbolic fringes of constructive/destructive interference).  
- **Four sources in a square:** rich 2-D interference with symmetry.  
- **$\alpha = 0$:** wavefronts are equally bright near and far.  
- **$\alpha = 2$:** sources become "spotlights" that fade quickly.
