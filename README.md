# Engineering-Design-Labs

[cite_start]This repository contains a collection of four engineering laboratory projects completed for **PHYS 222**[cite: 1, 83, 144, 232]. [cite_start]The projects cover high-speed data acquisition, signal processing using Op-Amps, and heat transfer simulations using both empirical measurements and finite difference approximations[cite: 3, 75, 85, 146, 234].

## Lab 1: Transient Heat Conduction in a Fin
* [cite_start]**Objective:** Simulate transient heat conduction by cooling a steel nail in ice water and recording temperature decay at the top[cite: 234, 236].
* [cite_start]**Hardware:** Arduino, temperature sensor, and a steel nail[cite: 235, 236].
* [cite_start]**Calculations:** * Determined convective heat transfer coefficient ($\overline{h}$) as $59.84 \text{ W/m}^2\text{K}$[cite: 294].
    * [cite_start]Calculated thermal diffusivity ($\alpha$) as $1.008 \cdot 10^{-5} \text{ m}^2/\text{s}$[cite: 308].
* [cite_start]**Results:** Experimental values matched published ranges for steel ($4.2 \cdot 10^{-6}$ to $1.88 \cdot 10^{-5} \text{ m}^2/\text{s}$)[cite: 309, 310].

## Lab 2: Finite Difference Approximation (Heat Equation)
* [cite_start]**Objective:** Use Excel to solve steady-state and transient heat equations for a square column[cite: 145, 147].
* [cite_start]**Steady-State:** Modeled a column with one $100^{\circ}\text{C}$ face and three $0^{\circ}\text{C}$ faces until stability was reached[cite: 147, 150].
* [cite_start]**Transient State:** Simulated the temperature profile of a $100^{\circ}\text{C}$ column submerged in $0^{\circ}\text{C}$ water over time[cite: 177].
* [cite_start]**Constraint:** Applied $\Delta x=1, \Delta y=1, \Delta t=1$, and $\alpha=0.062$ to satisfy the stability criteria[cite: 181, 182].

## Lab 3: Arduino Oscilloscope
* [cite_start]**Objective:** Transform an Arduino into a dual-channel oscilloscope to record $1000\text{ Hz}$ signals[cite: 83, 85].
* [cite_start]**Key Feature:** Modified the ADC prescaler (ADCSRA) to maximize sampling speed for high-frequency capture[cite: 116].
* [cite_start]**Data:** Collected 100 samples per channel at a 115200 baud rate using `micros()` for precise timing[cite: 87, 117].
* [cite_start]**Findings:** Successfully visualized signal periods of $\approx 1000\text{ }\mu\text{s}$[cite: 142].

## Lab 4: Arduino Function Generator
* [cite_start]**Objective:** Generate Square, Triangle, and Sine waves using Arduino and analog circuitry[cite: 1, 3].
* [cite_start]**Circuit Design:** Utilized TL081 Op-Amps in an integrator configuration to convert square waves into triangle and sine waves[cite: 46, 48, 77].
* [cite_start]**Analysis:** * **Triangle Wave:** Measured amplitude $\approx 2.17\text{V}$ (Theoretical: $2.1\text{V}$)[cite: 79, 80].
    * [cite_start]**Sine Wave:** Measured amplitude $\approx 1.00\text{V}$ (Theoretical: $0.90\text{V}$)[cite: 81, 82].
* [cite_start]**Theory:** Theoretical values were approximated using Fourier series expansions[cite: 75, 78].

---
[cite_start]**Authors:** Eric Chen, Ethan Yang [cite: 2, 84, 144, 233]
