# Mini CAN FD Hat (40-Pin)

---

<details markdown="1">
  <summary>Table of Contents</summary>

<!-- TOC -->
* [Mini CAN FD Hat (40-Pin)](#mini-can-fd-hat-40-pin)
  * [1 Overview](#1-overview)
  * [2 Board Specifications](#2-board-specifications)
    * [2.1 Connectors](#21-connectors)
    * [2.2 Switches & Jumpers](#22-switches--jumpers)
  * [3 Schematics](#3-schematics)
<!-- TOC -->

</details>

---

## 1 Overview

---

## 2 Board Specifications

### 2.1 Connectors

Connectors fixed by hardware (PCB traces or the connector itself).

| Connector | Ref | Description                                    |
|-----------|:---:|------------------------------------------------|
| `40-pin`  | J1  | Standard 40-pin (2x20) GPIO pin header         |
| `CAN`     | J2  | Pin 1: ground, Pin 2: CAN high, Pin 3: CAN low |

### 2.2 Switches & Jumpers

User controllable hardware and/or firmware driven inputs.

| Switch/Jumper     | Ref | Description                                         |
|-------------------|:---:|-----------------------------------------------------|
| `CAN termination` | SW1 | 1 + 2 = 120 Ohm termination, 2 + 3 = No termination |
| `CAN silent`      | JP1 | Open = normal operation, closed = silent mode       |

---

## 3 Schematics

Download PDF: [can_hat_40_pcb-schematic.pdf](docs/can_hat_40_pcb-schematic.pdf).

![can_hat_40_pcb-schematic-1.png](docs/can_hat_40_pcb-schematic/can_hat_40_pcb-schematic-1.png)
