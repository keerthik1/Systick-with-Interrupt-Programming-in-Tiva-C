# SysTick Programming Using Interrupts on TIVA C LaunchPad

## Overview
This project demonstrates the use of the SysTick timer with interrupts on the TIVA C LaunchPad (EK-TM4C123GXL, TM4C123GH6PM microcontroller). The SysTick timer is configured to generate periodic interrupts at a 1 Hz frequency, toggling the onboard red LED (PF1) to indicate timing events. The project showcases embedded systems skills, including timer configuration, interrupt handling, and GPIO control, with applications in real-time systems and event scheduling.

### Features
- Configures the SysTick timer to generate interrupts every 1 second.
- Toggles the onboard red LED (PF1) at a 1 Hz frequency using SysTick interrupts.
- Sets the system clock to 16 MHz for accurate timing.
- Implements a simple counter to track elapsed time in seconds.
- Provides a modular interrupt handler for easy integration with other applications.

## Hardware Requirements
- **TIVA C LaunchPad**: EK-TM4C123GXL with TM4C123GH6PM microcontroller.
- **Onboard Components**:
  - Red LED: Connected to PF1 (part of the onboard RGB LED).
- **Optional External Components**:
  - External LED (with a 330-ohm resistor) for additional testing.
  - Connections (if using external LED):
    - External LED Anode → PA2 (or any GPIO pin)
    - External LED Cathode → GND (via resistor)

## Software Requirements
- **Code Composer Studio (CCS)**: Version 12.4.0 or later.
- **TivaWare**: Optional (this project uses direct register access for educational purposes).
- **Compiler**: TI ARM Compiler (included with CCS).

## Setup Instructions
1. **Hardware Setup**:
   - No additional connections are needed if using the onboard blue LED (PF2).
   - If using an external LED, connect it to PA2 (or another GPIO pin) as described above.
   - Power the LaunchPad via USB.
2. **Software Setup**:
   - Clone or download this repository.
