# Embedded Hardware Design Library

A collection of reusable embedded hardware designs developed as a personal reference library for future electronics and embedded-systems projects.

This repository contains custom development boards, microcontroller platforms, and DC-DC power-conversion designs. The goal is to maintain a structured library of proven circuit designs that can be reused, adapted, and expanded for future projects.

The designs emphasize **practical PCB implementation, component selection, power integrity, signal integrity, manufacturability, and reusable hardware architecture**.

This repository also serves as an ongoing engineering and learning platform. Designs are developed, evaluated, and refined to strengthen practical skills in embedded systems, PCB design, power electronics, signal integrity, and hardware validation. Lessons learned from each design are incorporated into subsequent revisions and projects.

---

## Repository Contents

### Microcontroller Development Boards

| Platform      | MCU                              | Primary Focus                                              |
| ------------- | -------------------------------- | ---------------------------------------------------------- |
| ATtiny1616    | Microchip ATtiny1616             | Low-cost / low-power embedded control                      |
| ATmega32U4    | Microchip ATmega32U4             | USB-capable embedded applications                          |
| ESP32-S3      | Espressif ESP32-S3               | Wi-Fi / Bluetooth / high-performance embedded applications |
| RP2040        | Raspberry Pi RP2040              | Dual-core MCU development                                  |
| STM32F103C8T6 | STMicroelectronics STM32F103C8T6 | ARM Cortex-M3 embedded development                         |

### Power Electronics

The repository also contains several DC-DC converter reference designs:

* Buck converter
* Boost converter
* SEPIC converter

These designs are intended as reusable starting points for future power-supply requirements, with component values and operating parameters selected for their respective target applications.

---

## Design Philosophy

The primary objective of this repository is **reusability**.

Rather than designing every development board or power stage from scratch, commonly used circuits are maintained as modular reference designs that can be incorporated into future projects.

Designs are developed with consideration for:

* Component availability
* PCB manufacturability
* Power distribution
* Decoupling and bypassing
* Signal integrity
* Grounding and return paths
* Programming and debugging interfaces
* Protection circuitry
* Ease of modification and reuse

---

## Development Boards

### ATtiny1616

Reference development board centered around the Microchip ATtiny1616 microcontroller.

Design considerations include:

* USB-to-serial conversion
* Programming/debug interface
* GPIO accessibility
* External power input
* Reset/programming provisions

### ATmega32U4

USB-capable development board based on the ATmega32U4.

The design provides a reusable platform for projects requiring:

* Native USB
* GPIO expansion
* Embedded control
* HID applications
* External peripherals

### ESP32-S3

Development platform based on the ESP32-S3 for projects requiring greater processing capability and wireless connectivity.

The design focuses on providing a reusable hardware platform while accounting for the additional power, RF, and high-speed considerations associated with the device.

### RP2040

Development board based on the Raspberry Pi RP2040.

The design provides a flexible platform for embedded applications requiring:

* Dual-core processing
* High-speed GPIO
* Programmable I/O
* USB connectivity
* External peripheral interfaces

### STM32F103C8T6

ARM Cortex-M3 development platform based on the STM32F103C8T6.

The design provides a compact reference platform for applications requiring:

* ARM Cortex-M development
* General-purpose peripherals
* Multiple communication interfaces
* External debugging/programming

---

## Power Conversion

### Buck Converter

Step-down DC-DC converter designs for applications requiring a regulated output voltage below the input voltage.

Design considerations include:

* Switching frequency
* Inductor selection
* Output capacitance
* MOSFET selection
* Diode or synchronous rectification
* Feedback network
* Switching losses
* Thermal performance
* PCB current paths

### Boost Converter

Step-up DC-DC converter designs for generating an output voltage greater than the input voltage.

Key considerations include:

* Inductor selection
* Switching device selection
* Diode characteristics
* Output ripple
* Duty-cycle limitations
* Feedback and regulation
* Current requirements

### SEPIC Converter

Single-Ended Primary-Inductor Converter designs for applications requiring an output voltage that may be either above or below the input voltage.

SEPIC designs are particularly useful when the input voltage can cross the desired output voltage while maintaining a non-inverting regulated output.

---

## Design Documentation

Each design is intended to become increasingly self-documenting as the repository develops.

Where applicable, documentation will include:

* Design objectives
* Electrical specifications
* Schematic
* PCB layout
* Bill of materials
* Component selection rationale
* Design calculations
* Simulation results
* PCB fabrication files
* Assembly information
* Bring-up and validation notes
* Known limitations
* Revision history

Measured results will be distinguished from simulated or calculated values.

---

## Tools

The designs in this repository may utilize:

* **KiCad** — Schematic capture and PCB design
* **LTspice** — Circuit simulation
* **Datasheet analysis** — Component selection and electrical verification
* **Embedded development tools** — Firmware development and hardware bring-up

Additional tools may be added as the library expands.

---

## Future Development

Planned additions and improvements include:

* Additional MCU development boards
* Expanded DC-DC converter library
* Reusable power-entry circuits
* USB interface designs
* Debug/programming interfaces
* ESD and transient protection circuits
* Load-switch and power-management circuits

---

## Status

This repository is an actively evolving engineering reference library.

Designs should be considered **development/reference hardware unless explicitly marked as validated**. Electrical specifications, component selections, and layouts may change as designs are tested and refined.
