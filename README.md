# EEE3088F 2025 - Power Subsystem Design

This repository contains the design and development files for the Power Subsystem of the Micro-Mouse (MM) Project, as part of the EEE3088F 2025 Course at UCT.

## Project Overview
The goal of this project is to collaboratively design and manufacture a custom PCB-based power module that will meet the electrical and mechanical requirements of the MM. Each group member is responsible for specific components of the design, and the system will be demonstrated as a team while reports are submitted individually.

## System Requirements
The power subsystem must:
- **Support 4 Motors:** 
  - 2x Brushed DC motors (200mA max each at full battery voltage).
  - 2x Auxiliary motors (500mA max each).
- **Battery Monitoring:** Integrate an INA219 sensor on the I2C bus with proper address configuration.
- **Battery Charging:** 
  - Charge from a 9V input.
  - Offer dual charging modes (200mA and ~600mA ±100mA).
- **Power Output:**
  - USB-C support with 9V output from the USB Host.
  - Two high-side external load switches (1A each, 5V rail).
  - 3.3V output with 5% accuracy (max 300mA).
  - 5V output with 5% accuracy (max 1.5A).
- **Power Control:** 
  - ON/OFF switch: OFF state <30uA draw, ON state can handle peak 2A.
  - Switch must cut 3.3V and 5V rails.

## Hardware Integration
- **Battery Connector:** JST PH 2mm pitch.
- **Main Connector:** 2x16 (2.54mm pitch) header to interface with the MM motherboard.
- **PCB Size Constraint:** Maximum dimensions 82mm x 60mm.
- **Shape Consideration:** The PCB must avoid interfering with motherboard drill holes.

