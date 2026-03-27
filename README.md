# Low-Power Single-Phase Transformer Design

This repository contains the mathematical design and component selection process for a low-power single-phase transformer. Developed as an academic project for the **Passive Components and Circuits (CCP)** course at ETTI, UNSTPB.

## About the Project
The goal of this project is to fully design a custom transformer from the ground up to power three distinct resistive networks using Through-Hole Technology (THT) components. The design accounts for environmental temperatures between 10°C and 80°C.

## Technical Specifications
* **Primary Winding:** 230V, 50Hz
* **Secondary 1 (11V):** Powers a complex resistive network (Wheatstone bridge).
* **Secondary 2 (14V):** Powers a circuit containing a resistor and an NTC thermistor (R25 = 33 ohms, B = 3000K).
* **Secondary 3 (150V):** Powers an RC series circuit (C1 = 2.2µF).

## Engineering & Design Process
The documentation covers the entire hardware engineering workflow:
1. **Circuit Analysis:** Calculating currents and dissipated power for each component, including a Delta-Wye transformation to solve the bridge circuit in Secondary 1.
2. **Component Selection (Derating):** Choosing physical THT resistors and capacitors based on calculated power. This includes applying derating principles (selecting components with roughly double the calculated power capacity to ensure thermal safety).
3. **Transformer Sizing:**
   * Calculating the total absorbed power (~42.42W).
   * Determining the required core cross-section (Standard E12.5 core selected without insulation between layers).
   * Calculating the turns ratio and standardized wire diameters for both primary and secondary windings.

## Full Documentation
For the complete mathematical calculations, schematic diagrams, technological execution details, and the final Bill of Materials (BOM), please see the attached Romanian documentation: `Necula_Adrian_Nicusor_422Ea.pdf`.
