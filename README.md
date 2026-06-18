# Active Bandpass Filter Circuit Design Project

## Overview
This group project details the design, simulation, and hardware implementation of an **Active Bandpass Filter Circuit** using the classic **LM741 Operational Amplifier (Op-Amp)**. The project bridges theoretical design with practical results through rigorous software simulation and physical bench testing.

## Component Specifications
The circuit was constructed using the following components:
* **Active Element:** LM741 Op-Amp
* **Resistors:** 2.2 kΩ, 5.6 kΩ
* **Capacitors:** 1 nF, 4.7 nF

---

## Phase 1: Software Simulation (PSpice for TI)
Before hardware assembly, the circuit was modeled and analyzed using **PSpice for TI** software. 

1. **Theoretical Calculation:** The center (resonant) frequency ($f_0$) was calculated to establish baseline expectations.
2. **Simulation Profiles:** A total of six simulation profiles were executed to analyze the circuit's behavior:
   * **AC Sweep Simulation (1 Profile):** Conducted to map the general frequency response and visualize the bandwidth of the filter.
   * **Time-Domain / Transient Simulations (5 Profiles):** Conducted at strategic frequency checkpoints to observe input vs. output waveforms:
     * $f < f_{\text{Low}}$ (Below the lower cut-off frequency)
     * $f = f_{\text{Low}}$ (At the lower cut-off frequency)
     * $f = f_0$ (At the center/resonant frequency)
     * $f = f_{\text{High}}$ (At the higher cut-off frequency)
     * $f > f_{\text{High}}$ (Above the higher cut-off frequency)

---

## Phase 2: Hardware Implementation & Testing
Following successful simulations, the physical circuit was built and verified:
* **Assembly:** Built on a standard solderless breadboard.
* **Input Generation:** A function generator was utilized to sweep through different input frequencies.
* **Measurement & Analysis:** An oscilloscope was connected to simultaneously monitor both the input and output signals, allowing for real-time comparison across the frequency spectrum.

## Conclusion
The physical hardware testing yielded experimental data that closely aligned with the initial PSpice simulation results, validating the accuracy of both the design calculations and the physical implementation.
