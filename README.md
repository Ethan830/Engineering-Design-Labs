# Engineering-Design-Labs

A collection of PHYS 222 engineering design labs by Eric Chen and Ethan Yang, featuring Arduino-based signal processing, high-speed data acquisition, and heat transfer simulations using finite difference approximations.

## Lab 1: Transient Heat Conduction in a Fin
* **Objective:** Simulate transient heat conduction by cooling a steel nail in ice water and recording temperature decay at the top.
* **Hardware:** Arduino, temperature sensor, and a steel nail.
* **Calculations:** * Determined convective heat transfer coefficient ($\overline{h}$) as $59.84 \text{ W/m}^2\text{K}$.
  * Calculated thermal diffusivity ($\alpha$) as $1.008 \cdot 10^{-5} \text{ m}^2/\text{s}$.
* **Results:** Experimental values matched published ranges for steel ($4.2 \cdot 10^{-6}$ to $1.88 \cdot 10^{-5} \text{ m}^2/\text{s}$).

## Lab 2: Finite Difference Approximation (Heat Equation)
* **Objective:** Use Excel to solve steady-state and transient heat equations for a square column.
* **Steady-State:** Modeled a column with one $100^\circ\text{C}$ face and three $0^\circ\text{C}$ faces until stability was reached.
* **Transient State:** Simulated the temperature profile of a $100^\circ\text{C}$ column submerged in $0^\circ\text{C}$ water over time.
* **Constraint:** Applied $\Delta x=1$, $\Delta y=1$, $\Delta t=1$, and $\alpha=0.062$ to satisfy the stability criteria.

## Lab 3: Arduino Oscilloscope
* **Objective:** Transform an Arduino into a dual-channel oscilloscope to record $1000\text{ Hz}$ signals.
* **Key Feature:** Modified the ADC prescaler (ADCSRA) to maximize sampling speed for high-frequency capture.
* **Data:** Collected 100 samples per channel at a 115200 baud rate using `micros()` for precise timing.
* **Findings:** Successfully visualized signal periods of $\approx 1000\text{ }\mu\text{s}$.

## Lab 4: Arduino Function Generator
* **Objective:** Generate Square, Triangle, and Sine waves using Arduino and analog circuitry.
* **Circuit Design:** Utilized TL081 Op-Amps in an integrator configuration to convert square waves into triangle and sine waves.
* **Analysis:** * **Triangle Wave:** Measured amplitude $\approx 2.17\text{V}$ (Theoretical: $2.1\text{V}$).
  * **Sine Wave:** Measured amplitude $\approx 1.00\text{V}$ (Theoretical: $0.90\text{V}$).
* **Theory:** Theoretical values were approximated using Fourier series expansions.

---
