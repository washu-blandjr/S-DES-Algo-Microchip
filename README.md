# S-DES-Algo-Microchip
Final project for Digital IC Class. Done with Hussein A. and Nicole E.

# Simplified DES Encryption Microchip
**Transistor-Level CMOS Implementation in Cadence Virtuoso**

## Overview
Complete digital integrated circuit implementing the Simplified DES encryption algorithm 
in 0.6μm CMOS process. Designed for 10 MHz operation with 40-pin interface.

## Specifications
- **Process Technology**: 0.6μm CMOS (AMI process)
- **Supply Voltage**: 3.3V VDD
- **Die Size**: 1.5mm × 1.5mm (2.25 mm²)
- **Operating Frequency**: 10 MHz (characterized up to 20 MHz)
- **Pin Count**: 40 pins (8-bit input, 10-bit key, 8-bit output, control, power)
- **Verification**: 100% DRC/LVS clean across all hierarchy levels

## Architecture
6-block hierarchical design:
- Key generation (k1/k2 subkey derivation)
- Initial permutation
- F-function rounds (2 stages with S-boxes)
- Inverse permutation
- Input/output registers with clock synchronization

## Design Highlights
- Custom transistor-level logic for XOR gates, S-boxes, and permutation networks
- Synchronous design with enable/disable control
- Optimized layout routing for 2.25mm² area constraint
- Python-based functional verification suite

## Tools
- Cadence Virtuoso (Schematic Capture, Layout, Simulation)
- Cadence Assura (DRC/LVS verification)
- Python (verification scripting)

## NOTE
This repo contains the files from our Digital Integrated Circuit final project. Me, Hussein A., and Nicole E. designed a plethora of schematics and layouts. The final result is a 1.5mm by 1.5mm, 40 pin microchip. When 1-bit enable is set to 1, and on a rising clock edge, the output from an 8-bit input, 10-bit key is displayed.
