# STM32-Based Industrial Conveyor Control System

<p align="center">
  <img src="docs/existing-system/conveyor-original-condition.jpg" width="850">
</p>

<h3 align="center">
  Legacy Industrial Control Analysis & Embedded-System Modernization
</h3>

<p align="center">
  Independent Embedded Systems Project
</p>

<p align="center">

  <img src="https://img.shields.io/badge/STM32-Embedded-blue?style=for-the-badge&logo=stmicroelectronics&logoColor=white">

  <img src="https://img.shields.io/badge/Embedded%20C-Firmware-blue?style=for-the-badge&logo=c&logoColor=white">

  <img src="https://img.shields.io/badge/PLC-Industrial%20Automation-orange?style=for-the-badge">

  <img src="https://img.shields.io/badge/Proteus-Circuit%20Simulation-red?style=for-the-badge">

  <img src="https://img.shields.io/badge/Fritzing-Hardware%20Design-green?style=for-the-badge">

</p>

---

## ⚙️ Project Overview

This project focuses on the analysis and modernization of an existing industrial conveyor control system.

The work began with an existing conveyor installation that was no longer operational. Instead of treating the equipment simply as a broken system, it was approached as an engineering problem: understanding the existing architecture, studying the legacy control system, identifying its limitations, and investigating a modern embedded alternative.

The project combines:

**Industrial Automation · Embedded Systems · Electronics · Sensor Interfacing · Actuator Control · Control Logic · Hardware Prototyping · Circuit Simulation**

---

## 🎯 Project Motivation

The project started from the observation of an existing conveyor system requiring investigation after becoming non-operational.

The first objective was to understand **how the original system worked** before considering any modification.

The investigation therefore focused on:

- Understanding the physical conveyor mechanism
- Identifying the role of the existing PLC
- Studying the connected sensors and actuators
- Understanding the control sequence
- Identifying practical limitations of the existing installation
- Investigating an STM32-based embedded alternative

> **Engineering question:**  
> How can the essential functions of an existing industrial control system be understood and modernized using embedded-system technology?

---

# 🏭 Existing Industrial System

## Telemecanique TSX07 PLC

The original conveyor control architecture was based on a **Telemecanique TSX07 PLC**.

The controller documented during the project was the:

**Telemecanique TSX07311622 TSX Nano Modicon**

The PLC formed part of the original control architecture, processing system inputs and controlling the corresponding outputs involved in the conveyor mechanism.

<p align="center">
  <img src="docs/existing-system/tsx07-plc-module.jpg" width="700">
</p>

### 🔎 Existing-System Investigation

The legacy control system was studied to understand:

| Area | Investigation |
|---|---|
| 🧠 Controller | Telemecanique TSX07 PLC |
| 📥 Inputs | Sensors and system signals |
| 📤 Outputs | Actuator/control signals |
| ⚙️ Mechanism | Conveyor operation |
| 🔌 Interfaces | Electrical connections |
| 🔄 Logic | Operating sequence |

---

# ⚠️ Why Investigate Modernization?

The existing installation presented several practical limitations.

### Identified constraints

- Limited access to the original PLC program
- Difficulty obtaining the required programming/connection cables
- Dependence on manual intervention for motor start/stop
- Legacy hardware and associated maintenance constraints

These limitations motivated the investigation of a **microcontroller-based control architecture**.

The objective was not simply to replace a PLC with a microcontroller.

The objective was to first understand the existing system and then determine how its essential control functions could be reproduced using an embedded architecture.

---

# 🔄 System Modernization Approach

The project followed a progressive engineering workflow:

```text
┌─────────────────────────────┐
│    Existing Conveyor        │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│  Telemecanique TSX07 PLC    │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│   Existing-System Analysis  │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│ Identify System Limitations │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│ Embedded-System Redesign    │
└──────────────┬──────────────┘
               │
               ▼
       ┌────────────────┐
       │ STM32 Control  │
       └───────┬────────┘
               │
       ┌───────┼────────┐
       ▼       ▼        ▼
   Sensors   Logic   Actuators
       │       │        │
       └───────┼────────┘
               ▼
┌─────────────────────────────┐
│ Simulation & Prototyping    │
└─────────────────────────────┘
