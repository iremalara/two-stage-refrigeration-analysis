# Thermodynamic and Exergetic Analysis of a Two-Stage Vapor Compression Refrigeration Cycle

## Abstract
This project presents a comprehensive thermodynamic model of a two-stage vapor compression refrigeration cycle developed using **Engineering Equation Solver (EES)**. The primary objective is to evaluate and compare the energy and exergy performances of the traditional R22 refrigerant against new-generation, low-GWP (Global Warming Potential) alternatives: **R1234yf, R227ea, and R600** 
### System Diagram
![Two-Stage Refrigeration System Schema](system_schema.png)

By conducting parametric studies under varying evaporator (-15°C to 5°C) and condenser (30°C to 50°C) temperatures, the study analyzes critical system outputs including Coefficient of Performance (COP), compressor power distribution, and cooling capacity. Furthermore, a detailed **Second Law (Exergy) analysis** is performed to pinpoint the exact locations and magnitudes of thermodynamic irreversibilities (exergy destruction) across system components. The findings provide a robust engineering framework for selecting optimum, environmentally sustainable refrigerants without compromising industrial system efficiency.


## System Parameters and Assumptions

The thermodynamic modeling and simulations were conducted under steady-state conditions[cite: 1]. The fundamental design parameters and reference operating conditions used in the EES model are summarized below:

| Parameter | Symbol | Value | Unit |
| :--- | :---: | :---: | :---: |
| Reference Evaporation Temperature | T_1 | -3 | °C |
| Reference Condensation Temperature | T_5 | 37 | °C |
| Total Mass Flow Rate | m_total | 0.1 | kg/s |
| Isentropic Efficiency of Compressors | η_LP, η_HP | 82 | % |
| Dead State Temperature (For Exergy) | T_0 | 20 | °C |
| Dead State Pressure (For Exergy) | P_0 | 101.3 | kPa |
| Reference Refrigerant | - | R22 | - |
| Alternative Refrigerants | - | R1234yf, R227ea, R600 | - |

### T-s Diagram (R22 Reference)
![T-s Diagram of the Refrigeration Cycle](ts_diagram.png)

**Key System Assumptions:**
* The system operates under steady-flow and steady-state conditions.
* Pressure drops in the connecting pipelines and heat transfer to/from the surroundings are neglected.
* The refrigerant exits the evaporator, condenser, and enters the low-pressure compressor in a completely saturated state (saturated vapor or saturated liquid).
* The expansion processes through the expansion valves are assumed to be isenthalpic.
* The mixing chamber and flash chamber are considered perfectly insulated (adiabatic).



## Key Findings & Conclusions

Based on the parametric energy and exergy analyses conducted in EES, the following principal conclusions were drawn:

* **Optimum Eco-Friendly Alternative (R1234yf):** R1234yf proved to be the most ideal sustainable replacement for R22, exhibiting only a negligible 0.64% decrease in Coefficient of Performance (COP). It offers a seamless transition for existing mechanical infrastructures without causing any performance degradation in terms of irreversibility management.
* **Maximum Efficiency but High Workload (R600):** Isobutane (R600) achieved the highest COP (3.68% increase over R22) and maximum cooling capacity due to its high latent heat of vaporization. However, it also required the highest compressor work, demanding larger system sizing.
* **Major Sources of Irreversibility:** The exergy analysis revealed that the majority of thermodynamic losses occur in the heat exchangers. Under standard design conditions for R22, the Evaporator accounts for 41% and the Condenser accounts for 35% of the total system exergy destruction.
  
### Exergy Destruction Distribution
![Exergy Destruction Ratio in System Components](exergy_chart.png)
  
* **Dynamic Exergy Behavior:** While the condenser's exergy destruction remains relatively stable, the exergy destruction in the evaporator accelerates exponentially when the system is pushed to lower evaporation temperatures (below -3°C).
* **Second Law Efficiency Trend:** As the evaporation temperature approaches the ambient temperature, the required mechanical work decreases (increasing actual COP); however, the "quality" of the cooling drops, resulting in a decrease in the Second Law (Exergetic) Efficiency.








