# Book Chapter - FPGA Based Solar Powered EV Charging Station: Smart Infrastructure for a Sustainable Future

> A book chapter presenting an FPGA-based solar powered electric vehicle charging station — covering FSM-based charge control, MPPT algorithm implementation, power routing logic, and environmental impact analysis — accepted for publication in CRC Press / Taylor & Francis Group.

![Status](https://img.shields.io/badge/Status-Accepted%20for%20Publication-brightgreen)
![Type](https://img.shields.io/badge/Type-Book%20Chapter-blue)
![Publisher](https://img.shields.io/badge/Publisher-CRC%20Press%20%2F%20Taylor%20%26%20Francis-orange)
![ISBN](https://img.shields.io/badge/ISBN-9781041093626-green)
![Signed](https://img.shields.io/badge/Agreement%20Signed-February%202026-brightgreen)
![Tool](https://img.shields.io/badge/Tool-Verilog%20HDL-purple)
![Tool](https://img.shields.io/badge/Tool-ModelSim-blue)



## 📄 Publication Details

| Field | Details |
|:---|:---|
| **Chapter Title** | FPGA Based Solar Powered EV Charging Station: Smart Infrastructure for a Sustainable Future |
| **Book Title** | Smart Technologies for Smart Buildings |
| **Publisher** | CRC Press, Taylor & Francis Group |
| **ISBN** | 9781041093626 |
| **Publication Agreement Signed** | February 2026 |
| **Status** | Accepted — Awaiting Publication |
| **Chapter Number** | Chapter 6 |



## 👥 Authors

| Name | ORCID | Affiliation |
|:---|:---|:---|
| Nakul S | [0009-0004-3319-7580](https://orcid.org/0009-0004-3319-7580) | VIT Chennai |
| **Preetham SK** | [0009-0003-0730-5384](https://orcid.org/0009-0003-0730-5384) | VIT Chennai |
| Pradeesh R | [0009-0007-7308-6764](https://orcid.org/0009-0007-7308-6764) | VIT Chennai |
| Kartheesan K | [0009-0005-4219-7520](https://orcid.org/0009-0005-4219-7520) | VIT Chennai |

*Research conducted under Dr. O.V. Gnana Swathika, Centre for Smart Grid Technologies (CSGT), VIT Chennai*



## 🔍 Overview

The rapid growth of electric vehicle (EV) adoption is placing unprecedented demand on charging infrastructure — requiring solutions that are efficient, reliable, grid-friendly, and environmentally sustainable. Traditional EV charging systems using microcontroller or DSP-based control face limitations in real-time responsiveness, scalability, and energy management capability.

This chapter presents a comprehensive study of **FPGA-based Solar Powered EV Charging Stations** — exploring how Field Programmable Gate Arrays, combined with photovoltaic energy generation, can deliver intelligent, deterministic, and reconfigurable control for next-generation sustainable charging infrastructure.



## 🧠 Problem Addressed

Conventional EV charging infrastructure exhibits three critical limitations:

**1. Grid Overloading During Peak Demand:** Unmanaged charging creates synchronised demand spikes that strain grid infrastructure — particularly as EV penetration increases. Intelligent load scheduling and real-time demand response are essential to prevent localised grid failures.

**2. Inefficient Solar Integration:** Integrating PV generation with EV charging requires Maximum Power Point Tracking (MPPT) algorithms that can respond dynamically to irradiance and temperature variations. Microcontroller-based MPPT systems are too slow for rapid irradiance transients — losing recoverable solar energy.

**3. Battery Health and Charging Efficiency:** Fixed charging profiles accelerate battery degradation. Temperature-aware adaptive charging algorithms — requiring sub-millisecond control loops — are needed to prolong battery life while maintaining fast charging capability.



## 💡 FPGA Advantages for EV Charging Control

FPGAs provide deterministic parallel processing with sub-microsecond latency — enabling capabilities that software-based controllers cannot match:

- **Real-time MPPT** — FPGA-implemented Perturb & Observe algorithm adjusts converter duty cycles faster than irradiance transients, maximising PV energy harvest
- **Adaptive Load Scheduling** — FPGA schedulers reduce peak demand by 15% while maintaining power factor >0.95
- **8× faster decisions** than PLC-based systems
- **Temperature-aware charging** — Reflex charge control suppresses battery temperature rise by 2–3°C, directly extending battery cycle life
- **Hardware-level cybersecurity** — FPGA-based encryption secures communication without latency penalties



## ⚙️ Implementation

### 1. FSM-Based Charge Controller
An 11-state Finite State Machine (FSM) was designed in Verilog HDL to manage the complete charging lifecycle:

| State | Function |
|:---|:---|
| IDLE | Awaiting vehicle connection |
| VEHICLE_DETECTED | EV presence confirmed, initiating communication |
| AUTHENTICATION | Verifying charging authorization |
| SOLAR_CHECK | Evaluating available PV power |
| MPPT_ACTIVE | Maximum Power Point Tracking active |
| PRE_CHARGE | Low-current pre-conditioning phase |
| FAST_CHARGE | High-current constant current phase |
| TAPER_CHARGE | Constant voltage tapering phase |
| TEMPERATURE_CHECK | Thermal monitoring and throttling |
| FAULT_DETECTION | Overcurrent / overvoltage / thermal fault handling |
| CHARGE_COMPLETE | Termination and disconnection sequence |

### 2. MPPT Algorithm — Perturb and Observe (P&O)
The Perturb & Observe MPPT algorithm was implemented to track the maximum power point of the PV array under variable irradiance conditions. The algorithm periodically perturbs the operating voltage and observes the resulting power change — adjusting the DC-DC converter duty cycle to maintain operation at the MPP.

Functional simulation and waveform verification performed using ModelSim — validating correct state transitions across all operating scenarios including partial shading and rapid irradiance changes.



## 📊 Key Results

| Metric | Value |
|:---|:---|
| **Peak demand reduction** | 15% with FPGA scheduler |
| **Power factor maintained** | > 0.95 |
| **Decision speed vs PLC** | 8× faster |
| **Battery temperature suppression** | 2–3°C reduction (reflex charging) |
| **CO₂ reduction vs gasoline** | Up to 99.8% |
| **SO₂ reduction vs gasoline** | Up to 99.7% |
| **NOx reduction vs gasoline** | 100% |



## 🎯 Applications

- **Commercial EV Charging Stations** — Grid-connected solar FPGA charging hubs
- **Residential Solar EV Integration** — Home PV + EV charging with smart load management
- **Fleet Charging Infrastructure** — Large-scale coordinated charging for commercial EV fleets
- **Off-Grid Rural Charging** — Standalone solar FPGA chargers for remote areas
- **Smart Grid Integration** — Vehicle-to-Grid (V2G) capable charging with FPGA control


## 🔗 Related Work

| Output | Details |
|:---|:---|
| **Book Chapter** | CRC Press, Taylor & Francis — ISBN 9781041093626 |
| **Research Supervisor** | Dr. O.V. Gnana Swathika, CSGT, VIT Chennai |
| **Research Centre** | Centre for Smart Grid Technologies (CSGT), VIT Chennai |
| **Internship** | Summer Research Intern, CSGT, VIT Chennai (May–July 2025) |



## 🤝 Connect

| **Author** | Preetham SK |
|:---|:---|
| **ORCID** | [0009-0003-0730-5384](https://orcid.org/0009-0003-0730-5384) |
| **Programme** | B.Tech. Electrical and Electronics Engineering, VIT Chennai |
| **LinkedIn** | [linkedin.com/in/preethamsk16](https://www.linkedin.com/in/preethamsk16) |
| **GitHub** | [github.com/PreethamSK163](https://github.com/PreethamSK163) |
| **Portfolio** | [preethamsk163.github.io](https://preethamsk163.github.io) |
| **Email** | preethamsk163@gmail.com |
