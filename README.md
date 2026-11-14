
# Book Chapter — FPGA Based Solar Powered EV Charging Station: Smart Infrastructure for a Sustainable Future

> An FPGA-based solar-powered EV charging infrastructure study exploring Verilog-based digital control, FSM architecture, MPPT implementation, intelligent power management and programmable hardware for sustainable transportation.

![Status](https://img.shields.io/badge/Status-Accepted%20for%20Publication-brightgreen)
![Type](https://img.shields.io/badge/Type-Book%20Chapter-blue)
![Publisher](https://img.shields.io/badge/Publisher-CRC%20Press%20%2F%20Taylor%20%26%20Francis-orange)
![ISBN](https://img.shields.io/badge/ISBN-9781041093626-green)
![Agreement](https://img.shields.io/badge/Agreement%20Signed-February%202026-brightgreen)
![HDL](https://img.shields.io/badge/HDL-Verilog-purple)
![Simulation](https://img.shields.io/badge/Simulation-ModelSim-blue)

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

*Research conducted under Dr. O.V. Gnana Swathika, Centre for Smart Grid Technologies (CSGT), VIT Chennai.*

## 🔬 Relevance to Semiconductor Technology & Digital Hardware

This work demonstrates the application of programmable digital hardware to real-time energy management, providing practical experience in hardware description languages, digital architecture, control logic and functional verification.

Although FPGA implementation differs from standard-cell ASIC implementation, the underlying digital design concepts are relevant to semiconductor engineering and integrated-circuit development.

### 1. FPGA-Based Digital Hardware Architecture

- Developed an 11-state Finite State Machine using Verilog HDL for EV charging control.
- Structured the charging controller into dedicated digital control operations.
- Applied programmable logic to implement coordinated and deterministic system behaviour.

### 2. Hardware Description Language and RTL Design

- Used Verilog HDL to describe the charging controller and its operating logic.
- Developed sequential control logic and state-transition behaviour.
- Gained practical experience translating system-level requirements into synthesizable digital hardware descriptions.

### 3. Digital Control and Hardware-Oriented Algorithm Implementation

- Implemented Perturb and Observe (P&O) MPPT logic for photovoltaic power optimisation.
- Integrated control decisions with converter duty-cycle adjustment.
- Explored the implementation of algorithmic operations using digital hardware rather than relying exclusively on software execution.

### 4. Functional Verification

- Used ModelSim for Verilog-based functional simulation.
- Verified FSM state transitions and controller behaviour under different operating conditions.
- Evaluated the interaction between control logic and MPPT operations.

This project complements my ASIC-oriented VLSI experience by adding exposure to programmable hardware, digital control architecture and RTL verification, providing a broader foundation in digital semiconductor systems.

## 🔍 Overview

The growing adoption of electric vehicles is increasing the demand for charging infrastructure that is efficient, reliable and environmentally sustainable. Integrating photovoltaic energy generation with intelligent charging control offers a way to improve energy utilisation and reduce dependence on conventional grid power.

This chapter presents an **FPGA-Based Solar Powered EV Charging Station**, exploring the use of programmable hardware for charging control, Maximum Power Point Tracking (MPPT) and intelligent power management.

The work combines digital control architecture, Verilog-based implementation and functional simulation to investigate an intelligent charging infrastructure.

## 🧠 Problem Addressed

Conventional EV charging infrastructure faces several challenges:

- **Grid Demand Management:** Uncoordinated charging can increase peak electricity demand and place additional stress on distribution networks.
- **Solar Energy Utilisation:** Variations in solar irradiance and temperature require adaptive MPPT control to improve photovoltaic energy harvesting.
- **Battery Charging Management:** Charging systems require coordinated control and monitoring to support safe and efficient charging operation.
- **Real-Time Control:** Charging infrastructure requires reliable digital control to coordinate different operating states and respond to changing system conditions.

The proposed approach investigates FPGA-based control to address these challenges through deterministic digital logic and coordinated system operation.

## 💡 FPGA-Based Control Architecture

The chapter explores the use of FPGA technology for real-time EV charging management through:

- **FSM-Based Charge Control** — Managing charging states and operating sequences.
- **Perturb and Observe MPPT** — Tracking the photovoltaic array's maximum power point under changing operating conditions.
- **Power Management** — Coordinating solar power availability and charging operation.
- **Temperature Monitoring** — Supporting temperature-aware charging control.
- **Programmable Hardware** — Enabling deterministic and reconfigurable digital control.

## ⚙️ Hardware Design & Implementation

### 1. FSM-Based Charge Controller

An 11-state Finite State Machine (FSM) was developed using Verilog HDL to coordinate the charging lifecycle.

| State | Function |
|:---|:---|
| IDLE | Awaiting vehicle connection |
| VEHICLE_DETECTED | Detecting vehicle connection |
| AUTHENTICATION | Verifying charging authorization |
| SOLAR_CHECK | Evaluating available photovoltaic power |
| MPPT_ACTIVE | Executing maximum power point tracking |
| PRE_CHARGE | Managing the initial charging phase |
| FAST_CHARGE | Controlling the main charging phase |
| TAPER_CHARGE | Managing the final charging phase |
| TEMPERATURE_CHECK | Monitoring thermal conditions |
| FAULT_DETECTION | Handling abnormal operating conditions |
| CHARGE_COMPLETE | Managing charging termination |

### 2. MPPT Algorithm — Perturb and Observe

The Perturb and Observe (P&O) algorithm was implemented to track the maximum power point of the photovoltaic array.

The algorithm periodically adjusts the operating voltage and evaluates the resulting power variation. Based on this change, the controller updates the DC-DC converter duty cycle to move the PV system towards its maximum power operating point.

This provides practical exposure to translating an energy-management algorithm into digital control logic.

### 3. Functional Simulation and Verification

Verilog-based functional simulation was performed using ModelSim to verify:

- FSM state transitions and charging sequences.
- Controller behaviour under different operating conditions.
- MPPT-related control behaviour.
- Functional coordination between the digital control blocks.

## 📊 Key Results

The chapter discusses the following system-level outcomes:

| Metric | Reported Value |
|:---|:---|
| **Peak Demand Reduction** | 15% |
| **Power Factor** | > 0.95 |
| **Decision Speed vs. PLC** | 8× faster |
| **Battery Temperature Suppression** | 2–3°C reduction |
| **CO₂ Reduction vs. Gasoline** | Up to 99.8% |
| **SO₂ Reduction vs. Gasoline** | Up to 99.7% |
| **NOx Reduction vs. Gasoline** | 100% |

*Reported values are based on the study presented in the book chapter.*

## 🎯 Applications

- **Commercial EV Charging Stations** — Solar-powered charging infrastructure with intelligent control.
- **Residential Solar EV Integration** — Coordinated photovoltaic generation and home EV charging.
- **Fleet Charging Infrastructure** — Managed charging for commercial electric vehicle fleets.
- **Off-Grid Charging** — Solar-powered charging solutions for remote locations.
- **Smart Grid Integration** — Intelligent charging management and potential Vehicle-to-Grid (V2G) applications.

## 🔗 Related Work

| Output | Details |
|:---|:---|
| **Book Chapter** | CRC Press, Taylor & Francis — ISBN 9781041093626 |
| **Research Supervisor** | Dr. O.V. Gnana Swathika, CSGT, VIT Chennai |
| **Research Centre** | Centre for Smart Grid Technologies (CSGT), VIT Chennai |
| **Internship** | Summer Research Intern, CSGT, VIT Chennai (May–July 2025) |

## 🤝 Connect

| Platform | Link |
|:---|:---|
| **Author** | Preetham Senthil Kumar Kalpana (Preetham SK) |
| **ORCID** | [0009-0003-0730-5384](https://orcid.org/0009-0003-0730-5384) |
| **Programme** | M.Sc. Nanoelectronic Systems, TU Dresden · B.Tech. EEE, VIT Chennai |
| **LinkedIn** | [linkedin.com/in/preethamsk16](https://www.linkedin.com/in/preethamsk16) |
| **GitHub** | [github.com/PreethamSK163](https://github.com/PreethamSK163) |
| **Portfolio** | [preethamsk163.github.io](https://preethamsk163.github.io) |
| **Email** | skpreetham16@gmail.com |
