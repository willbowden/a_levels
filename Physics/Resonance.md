# Resonance
### Free And Forced Oscillations
- **Free oscillations** have a constant amplitude. A freely oscillating pendulum will swing at its particular, **natural frequency** with the same amplitude for all time.
- A periodic driving force will make the system oscillate at the frequency of the driving force (**driver frequency**), these are **forced oscillations**.

### Energy Of A Harmonic Oscillator
- Energy of an oscillator constantly shits between kinetic energy and elastic potential energy stored in the spring, or gravitational potential. 
- Therefore, the total energy of the oscillator = $E_{k} + E{p} = \frac{1}{2}kA^2$
- This is because when all the energy is in potential, displacement = A: $E_{T} = E{p} = \frac{1}{2}kx^2 = \frac{1}{2}kA^2$

![[Energy Of Simple Harmonic Oscillator.png]]
 
 ### Damping
 - A free oscillator will oscillate indefinitely, with the amplitude and the total energy remaining constant.
 - The oscillators we observe, such as pendulums, do not oscillate indefinitely. Energy gradually leaks away because of **damping** - the action of forces such as friction and air resistance.
 - **Light damping -** max displacement of an oscillator is reduced with each oscillation.
 - **Critically Damped -** oscillator stops at equilibrium position without completing a cycle.
 - **Heavily damped -** the oscillator returns to the equilibrium much more slowly than the above two scenarios.
 
 ![[SHO Damping.png]]
 
 ### Resonance
- Resonance occurs when the periodic frequency driving an oscillation matches the natural frequency (**resonant frequency**) of the oscillator.
- The amplitude of the oscillations will rise until the energy loss per cycle is equal to the energy supplied by the driver.
- If the system is only lightly damped, the increase in amplitude can be dramatic.
- With a driving frequency exceeding the natural frequency, the amplitude will be less than without a driver.
- In the below image, the oscillation machine adds a driving force to the string/pulley system, which causes the amplitude of the oscillations to increase.

 ![[Resonant Frequency.png]]
 
 ### More Equations
 > $E_k = E_T - E_p$
 > $\frac{1}{2}mv^2 = \frac{1}{2}kx^2$
 > $v^2 = \frac{k}{m}x^2$
 > $v^2 = \frac{k}{m}(A^2-x^2)$
 > $v = \sqrt{\frac{k}{m}}\sqrt{(A^2-x^2)}$
 > When displacement x = 0, velocity is at its maximum:
 > $v_{max} = \sqrt{\frac{k}{m}}\sqrt{(A^2)}$
 > $\frac{k}{m} = \omega^2$

### But why does $\frac{k}{m} = \omega^2$?

| Symbol   | Meaning                           |
| -------- | --------------------------------- |
| $-x_0$   | displacement due to 'mg' force    |
| $-x$     | displacement due to pulling force |
| $-x-x_0$ | displacement due to both forces   |

> Imagine a spring oscillator. Force due to tension in the spring:
> $F_T = mg = k(-x_0)$
> Restoring force R:
> $R = k(-x-x_0)$
> $ma = R + (-mg)$
> By substituting R into the ma equation:
> $ma = -kx$
> $a = (-\frac{k}{m})x$
> Now, we also know that:
> $a = -\omega^2 x$
> Therefore:
> $\omega^2 = \frac{k}{m}$