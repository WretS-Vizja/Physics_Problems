## 2. Harmonic Motion
 
A 10 kg mass is attached to a spring and oscillates according to the equation $x(t) = 0.2 \cos(10\pi t)$ (in meters). What is the spring constant $k$? What is the total mechanical energy of the system?
 
> **Idea**
>
> The general equation for simple harmonic motion is $x(t) = A\cos(\omega t + \phi)$. By comparing this with the given equation $x(t) = 0.2\cos(10\pi t)$, we can directly read off the amplitude $A$ and angular frequency $\omega$. For a spring-mass system, the angular frequency is related to the spring constant by $\omega = \sqrt{k/m}$, and the total mechanical energy (which is constant throughout the motion) equals the maximum potential energy.
 
> **Step 1 – Identify parameters by comparison**
>
> Comparing $x(t) = 0.2\cos(10\pi t)$ with $x(t) = A\cos(\omega t)$:
>
> $A = 0.2 \text{ m}$ (the maximum displacement from equilibrium)
>
> $\omega = 10\pi \text{ rad/s}$ (angular frequency)
>
> We can also find the ordinary frequency and period:
>
> $f = \dfrac{\omega}{2\pi} = \dfrac{10\pi}{2\pi} = 5 \text{ Hz}$ (5 oscillations per second)
>
> $T = \dfrac{1}{f} = 0.2 \text{ s}$ (each oscillation takes 0.2 seconds)
 
> **Step 2 – Find the spring constant**
>
> The defining relationship for a spring-mass oscillator is:
>
> $\omega = \sqrt{\dfrac{k}{m}}$
>
> Squaring both sides: $\omega^2 = \dfrac{k}{m}$
>
> Solving for $k$: $k = m\omega^2$
>
> Substituting:
>
> $k = 10 \times (10\pi)^2 = 10 \times 100\pi^2 = 1000\pi^2$
>
> $k \approx 1000 \times 9.8696 = 9869.6 \text{ N/m}$
>
> **Unit check:** $[\text{kg}][\text{rad/s}]^2 = \text{kg/s}^2 = \text{N/m}$ ✓
>
> **Physical note:** This is a very stiff spring (~9870 N/m). For context, a typical car suspension spring has $k \approx 10{,}000$–$30{,}000$ N/m, so this is in that ballpark.
 
> **Step 3 – Calculate the total mechanical energy**
>
> In SHM, energy constantly converts between kinetic and potential forms, but the total remains constant. The easiest way to find the total energy is to evaluate it at the amplitude, where the mass momentarily stops ($v = 0$), so all energy is potential:
>
> $E = \dfrac{1}{2}kA^2$
>
> Substituting:
>
> $E = \dfrac{1}{2} \times 1000\pi^2 \times (0.2)^2$
>
> $E = \dfrac{1}{2} \times 1000\pi^2 \times 0.04 = 20\pi^2$
>
> $E \approx 20 \times 9.8696 = 197.4 \text{ J}$
>
> **Alternative check using kinetic energy at equilibrium:** At $x = 0$, all energy is kinetic. The maximum velocity is $v_{max} = A\omega = 0.2 \times 10\pi = 2\pi$ m/s. Then $E = \frac{1}{2}mv_{max}^2 = \frac{1}{2}(10)(2\pi)^2 = 5 \times 4\pi^2 = 20\pi^2$ ✓ — the same result, confirming energy conservation.
 
> **Result**
>
> $\boxed{k = 1000\pi^2 \approx 9870 \text{ N/m}}$
>
> $\boxed{E = 20\pi^2 \approx 197.4 \text{ J}}$
 
---
