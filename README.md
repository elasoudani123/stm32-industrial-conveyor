<div align="center">

# STM32-Based Industrial Conveyor Control System

### Legacy Industrial Control Analysis & Embedded-System Modernization

<br>

<img src="docs/existing-system/conveyor-original-condition.jpg" width="700">

<br><br>

<p>
  <img src="https://skillicons.dev/icons?i=c&perline=1" />
</p>

<p>
  <b>STM32 · Embedded C · PLC · Telemecanique TSX07 · Proteus ISIS 8 · Fritzing</b>
</p>

</div>

---

## Overview

This project focuses on the analysis and modernization of an existing
industrial conveyor control system.

The project started from an existing conveyor installation that was no
longer operational. Rather than treating the equipment simply as a
broken machine, the system was approached as an engineering problem:
understanding the existing architecture, identifying the role of the
legacy controller and connected equipment, and investigating how the
control system could be approached using modern embedded-system
technology.

The work combines industrial automation, embedded systems, electronics,
sensor interfacing, actuator control, control logic, hardware
prototyping, and circuit simulation.

The project was developed as an independent engineering initiative,
with the objective of understanding and improving an existing system
rather than starting from a completely new installation.

---

# Project Objectives

The main objectives of the project were to:

- Investigate an existing industrial conveyor system
- Understand the role of the original PLC
- Study the sensors and actuators involved in the mechanism
- Analyze the existing operating sequence
- Identify practical limitations of the legacy control architecture
- Investigate an STM32-based embedded control alternative
- Develop and document the corresponding control logic
- Model the hardware architecture
- Use Proteus ISIS 8 for circuit simulation
- Use Fritzing for hardware prototyping and documentation

The project therefore combines both **system analysis** and
**embedded-system development**.

---

# Existing Industrial System

## Telemecanique TSX07 PLC

The original conveyor control architecture was based on a
**Telemecanique TSX07 PLC**.

The controller documented during the project was the:

**Telemecanique TSX07311622 TSX Nano Modicon**

<p align="center">
  <img src="docs/existing-system/tsx07-plc-module.jpg" width="650">
</p>

<p align="center">
  <em>Telemecanique TSX07 PLC used in the existing conveyor installation</em>
</p>

The PLC represented the original control layer of the system and was
studied in order to understand the relationship between the industrial
equipment, system inputs, outputs, and operating sequence.

### Existing System Analysis

| System Element | Role |
|---|---|
| TSX07 PLC | Original control system |
| Sensors | Detection and system inputs |
| Motor | Conveyor actuation |
| Control logic | Defines the operating sequence |
| Electrical interfaces | Connects sensors, controller and actuators |
| Conveyor mechanism | Physical process being controlled |

---

# Why Investigate a Modernized Architecture?

The existing installation presented several practical limitations.

The investigation identified issues including:

- Limited access to the original PLC program
- Difficulty obtaining the required PLC programming and connection
  cables
- Dependence on manual intervention for motor start/stop
- Legacy hardware and associated maintenance constraints

These limitations provided the motivation to investigate a
microcontroller-based control architecture.

The objective was not simply to replace the PLC because it was old.

The first step was to understand the existing system and determine which
functions would need to be reproduced or adapted in a modern embedded
architecture.

---

# System Modernization Approach

The project followed a progressive engineering approach:

```text
┌─────────────────────────────┐
│     Existing Conveyor       │
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
│ Embedded-System Approach    │
└──────────────┬──────────────┘
               │
               ▼
       ┌────────────────┐
       │ STM32 Control  │
       └───────┬────────┘
               │
       ┌───────┼────────┐
       ▼       ▼        ▼
    Sensors  Logic   Actuators
       │       │        │
       └───────┼────────┘
               ▼
┌─────────────────────────────┐
│ Simulation & Prototyping    │
└─────────────────────────────┘
