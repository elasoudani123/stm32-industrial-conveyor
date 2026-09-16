# STM32-Based Industrial Conveyor Control System

> Independent Embedded Systems Project — Legacy PLC Analysis & Microcontroller-Based Modernization

<p align="center">
  <img src="docs/existing-system/conveyor-original-condition.jpg" width="850">
</p>

<p align="center">
  <b>Investigation and modernization of an existing industrial conveyor control system.</b>
</p>

---

## Overview

This project focuses on the analysis and modernization of an existing industrial conveyor control system.

The work began with an existing conveyor installation that was no longer operational. The system was investigated from both the equipment and control perspectives in order to understand its existing architecture, identify practical limitations, and explore a modern embedded alternative.

The project combines industrial automation, embedded systems, sensor interfacing, actuator control, control logic, hardware prototyping, and circuit simulation.

---

## Project Motivation

The starting point was an existing conveyor system that required investigation after becoming non-operational.

Rather than treating the equipment simply as a broken system, the project approached it as an engineering problem:

> **How can an existing industrial control system be understood, redesigned, and modernized using embedded-system technology?**

The first stage therefore consisted of studying the existing equipment and its control architecture before considering an alternative implementation.

---

# Existing Industrial Control System

## Telemecanique TSX07 PLC

The original conveyor control system was based on a **Telemecanique TSX07 PLC**.

The controller documented during the project was the:

**Telemecanique TSX07311622 TSX Nano Modicon**

The PLC formed part of the original control architecture, processing system inputs and controlling the corresponding outputs involved in the conveyor mechanism.

<p align="center">
  <img src="docs/existing-system/tsx07-plc-module.jpg" width="700">
</p>

### Existing-System Investigation

Understanding the legacy controller was an important part of the project.

The investigation considered:

- The role of the PLC within the conveyor system
- The relationship between inputs and outputs
- The connected sensors and actuators
- The existing operating sequence
- Practical limitations affecting maintenance and modification

---

# Why Modernize the Control System?

The investigation identified several practical limitations associated with the existing installation.

These included:

- Limited access to the original PLC program
- Difficulty obtaining the required programming and connection cables
- Dependence on manual intervention for motor start/stop
- Legacy hardware and associated maintenance constraints

These limitations motivated the investigation of a microcontroller-based alternative.

The objective was not simply to replace a PLC with a microcontroller, but to understand the existing control architecture and determine how its essential functions could be reproduced using an embedded system.

---

# System Modernization

The modernization approach followed a progressive engineering process:

```text
Existing Conveyor
       │
       ▼
Telemecanique TSX07 PLC
       │
       ▼
Existing System Analysis
       │
       ▼
Identification of Limitations
       │
       ▼
Embedded System Redesign
       │
       ▼
STM32-Based Control
       │
       ├──────── Sensor Interface
       │
       ├──────── Control Logic
       │
       └──────── Actuator Control
       │
       ▼
Hardware Prototyping & Simulation
