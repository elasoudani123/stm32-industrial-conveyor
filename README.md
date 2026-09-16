# STM32-Based Industrial Conveyor Control System

<p align="center">
  <img src="docs/existing-system/conveyor-original-condition.jpg" width="850">
</p>

<p align="center">
  <strong>Legacy Industrial Control Analysis & Embedded-System Modernization</strong>
</p>

<p align="center">
  Independent Embedded Systems Project
</p>

<p align="center">
  <img src="https://img.shields.io/badge/STM32-Embedded%20Systems-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white">
  <img src="https://img.shields.io/badge/C-Embedded%20Programming-A8B9CC?style=for-the-badge&logo=c&logoColor=black">
  <img src="https://img.shields.io/badge/PLC-Industrial%20Automation-007ACC?style=for-the-badge">
  <img src="https://img.shields.io/badge/Proteus-Circuit%20Simulation-8A2BE2?style=for-the-badge">
  <img src="https://img.shields.io/badge/Fritzing-Hardware%20Design-FF6F00?style=for-the-badge">
</p>

---

## Overview

This project focuses on the analysis and modernization of an existing industrial conveyor control system.

The project began with an existing conveyor installation that was no longer operational. Instead of treating the equipment simply as a broken system, it was approached as an engineering problem: understanding the existing architecture, studying the legacy control system, identifying practical limitations, and investigating a modern embedded alternative.

The work combines:

**Industrial Automation · Embedded Systems · Electronics · Sensor Interfacing · Actuator Control · Control Logic · Hardware Prototyping · Circuit Simulation**

---

## Project Motivation

The starting point was an existing conveyor system requiring investigation after becoming non-operational.

The first objective was to understand **how the original system worked** before considering any modification.

The investigation therefore focused on:

- Understanding the physical conveyor mechanism
- Identifying the role of the existing PLC
- Studying the connected sensors and actuators
- Understanding the operating sequence
- Identifying practical limitations of the existing installation
- Investigating an STM32-based embedded alternative

> **Engineering Question**
>
> How can the essential functions of an existing industrial control system be understood and modernized using embedded-system technology?

---

# Existing Industrial Control System

## Telemecanique TSX07 PLC

The original conveyor control architecture was based on a **Telemecanique TSX07 PLC**.

The controller documented during the project was the:

**Telemecanique TSX07311622 TSX Nano Modicon**

The PLC formed part of the original control architecture, processing system inputs and controlling the corresponding outputs involved in the conveyor mechanism.

<p align="center">
  <img src="docs/existing-system/tsx07-plc-module.jpg" width="700">
</p>

<p align="center">
  <em>Existing Telemecanique TSX07 industrial controller</em>
</p>

### Existing-System Investigation

The legacy control system was studied from both the controller and equipment perspectives.

| Area | Focus |
|---|---|
| Controller | Telemecanique TSX07 PLC |
| Inputs | Sensors and system signals |
| Outputs | Actuator/control signals |
| Mechanism | Conveyor operation |
| Interfaces | Electrical connections |
| Logic | Operating sequence |

---

# Why Investigate Modernization?

The existing installation presented several practical limitations.

These included:

- Limited access to the original PLC program
- Difficulty obtaining the required programming and connection cables
- Dependence on manual intervention for motor start/stop
- Legacy hardware and associated maintenance constraints

These limitations motivated the investigation of a microcontroller-based control architecture.

The objective was not simply to replace a PLC with a microcontroller.

Instead, the project first examined the existing architecture and then investigated how its essential control functions could be approached using embedded-system technology.

---

# System Modernization

The modernization study followed a progressive engineering approach:

```text
Existing Conveyor
       │
       ▼
Telemecanique TSX07 PLC
       │
       ▼
Existing-System Analysis
       │
       ▼
Identification of Limitations
       │
       ▼
Embedded-System Redesign
       │
       ▼
STM32-Based Architecture
       │
       ├──────── Sensor Interface
       │
       ├──────── Control Logic
       │
       └──────── Actuator Control
       │
       ▼
Hardware Prototyping & Simulation
