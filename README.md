# Buck Converter

A DC-DC buck converter system for efficient voltage step-down, controlled via a microcontroller or timer IC.

## Features

- Adjustable output voltage through PWM control
- Efficient power conversion using MOSFET and Schottky diode
- Compact design with Kicad Schematic, PCB layout, and LTspice simulation

## Technologies

This project is built with:

- **Firmware**: Arduino (ESP32 or compatible microcontroller)
- **Hardware Design**: KiCAD (schematic and PCB)
- **Simulation**: LTspice

## Included Files

- **Control Code**: `Buck_Converter.ino` contains the microcontroller code for regulating the buck converter’s output voltage, interfacing with the NE555 timer or directly controlling the IRLZ44N MOSFET.
- **Schematic**: `Buck_Converter_Design.kicad_sch` provides the circuit schematic, including the NE555D timer, IRLZ44N MOSFET, 1N5819 Schottky diode, and 30.5 µH inductor.
- **PCB Layout**: `Buck_Converter.kicad_pcb` includes the PCB design for the buck converter circuit.
- **Simulation**: `Buck_Converter_LTspice_Simulation.asc` is an LTspice simulation file for analyzing the buck converter’s performance, including voltage regulation and switching behavior.

## Installation

Follow these steps to set up the firmware and hardware:

### Firmware

1. Open `Buck_Converter.ino` in the Arduino IDE.
2. Configure pin assignments and PWM parameters for your ESP32 or compatible microcontroller.
3. Upload the code to your microcontroller board.

### Hardware

1. Open `Buck_Converter_Design.kicad_sch` in KiCAD to review the schematic.
2. Use `Buck_Converter.kicad_pcb` to fabricate the PCB or assemble the circuit on a prototyping board.
3. Connect a 24V input power source as indicated in the schematic.

### Simulation

1. Open `Buck_Converter_LTspice_Simulation.asc` in LTspice.
2. Run the simulation to analyze the circuit’s performance, such as output voltage and current characteristics.
