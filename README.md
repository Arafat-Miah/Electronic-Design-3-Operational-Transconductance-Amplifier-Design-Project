# Design and Layout Verification of an Operational Transconductance Amplifier (OTA) in 45 nm CMOS

This repository contains my **Electronics Design III** course project on the **design, simulation, layout, and verification of an Operational Transconductance Amplifier (OTA)** using **Cadence Virtuoso** in **45 nm generic CMOS technology**.

## Project Overview

The goal of this project was to design an OTA according to given specifications, develop a suitable bias circuit, verify the design through simulation, and complete physical layout verification. The work included:

- Hand calculation-based initial transistor sizing
- Schematic design of the OTA and bias circuit
- DC, AC, and transient simulations
- Input common-mode and output range verification
- Matching-aware layout design
- DRC and LVS verification of the OTA, bias circuit, and integrated layout

## Given Design Specifications

- **Technology:** 45 nm generic CMOS
- **Supply Voltage:** 3 V
- **Load Capacitance:** 10 pF
- **Gain:** > 39 dB
- **Unity-Gain Bandwidth:** > 10 MHz
- **Slew Rate:** > 10 V/µs
- **Phase Margin:** > 60°
- **Output Linear Range:** 0.6 V to 2.2 V
- **Input Common-Mode Range:** 1.5 V to 2.3 V
- **Input-to-Output Current Ratio (K):** 2

## Design Flow

1. Hand calculation of transistor-level parameters and bias current
2. Schematic implementation of the OTA and bias circuit
3. DC simulation for operating points
4. AC simulation for gain, unity-gain bandwidth, and phase margin
5. Transient simulation for slew-rate verification
6. DC sweeps for input common-mode and output range verification
7. Layout implementation using matching-aware analog layout practices
8. DRC and LVS verification

## Final Simulation Results

The implemented design achieved the following results:

- **Unity-Gain Bandwidth (GBW):** 15.6 MHz
- **Slew Rate (SR):** 15.36 V/µs
- **Input Common-Mode Range:** 1.0 V to 2.25 V
- **Common-Mode Output Range:** 0.647 V to 2.32 V
- **Phase Margin:** ~71°

These results confirm stable operation and close agreement with the design targets.

## Layout and Verification Highlights

The layout was developed using analog layout good practices, including:

- Symmetric common-centroid placement for matched devices
- Short interconnects and shared diffusion where appropriate
- Proper PMOS/NMOS placement near supply rails
- DRC-clean layout
- LVS match between schematic and extracted layout

Verification was completed for:
- OTA layout
- Bias-circuit layout
- Integrated OTA + bias layout

## Important Note

Although the course assignment includes post-layout simulation using extracted parasitics, **post-layout simulation was not completed in this work due to time constraints**. However, the layout successfully passed **DRC** and **LVS**, confirming correct physical implementation and schematic equivalence.

## Repository Contents

- `report/` — accepted project report
- `assignment/` — original course design brief
- `images/` — optional project figures and screenshots

## EDA Tool Used

- **Cadence Virtuoso**
- **45 nm generic CMOS technology**

## Author

**Arafat Miah**  
MSc Electronics, University of Oulu
