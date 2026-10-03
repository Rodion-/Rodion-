# 📑 Rodion | Senior R&D Embedded Systems & Hardware Engineer

**Title:** Senior R&D Embedded Systems & Hardware Engineer | UAV Avionics & Power Electronics | Bare-Metal & FreeRTOS

**Location:** St. Petersburg, Russia (Available for 100% remote contract work worldwide)  
**Language for Tech Communication:** Written English (Fluent in datasheets, schematics, code, Slack, Jira, GitHub)  
**Hardware Capabilities:** Equipped with a private hardware laboratory (Rigol DS1102E 100MHz oscilloscope, Ersa Digital 2000 A professional SMD rework station, lab power supplies, logic analyzers) for independent local prototyping and debugging.

---

## 🚀 R&D PROFILE SUMMARY
Senior R&D engineer with a 14-year track record (since 2012) in full-cycle electronic product development, hardware architecture, and rapid prototyping. Expert in bridging the gap between heavy high-voltage power electronics, high-speed digital carrier boards, low-level firmware, and desktop software. Proven ability to architect and execute complex, cross-disciplinary systems single-handedly: from protocol reverse-engineering to multi-processor industrial UAV avionics and automated tracking gimbals. Fully autonomous developer who works directly at the register level for maximum efficiency and efficiency-critical systems.

---

## 🛠 TECHNICAL STACK & COMPETENCIES

*   **Microcontrollers & Firmware (Current Expert):** STM32 (F1, F3, F4, H7 series — primary expertise), NXP LPC, AVR ATmega. **Bare-metal expert** (direct register-level access, custom driver development from scratch without vendor HAL/SPL) & **FreeRTOS** architectures. Low-latency interrupt handling and precise timing optimization.
*   **Hardware Design & EDA (Current Expert):** Altium Designer (formerly P-CAD). High-density multi-layer PCB routing, signal integrity management for high-speed digital lines (Ethernet, processor buses), and **heavy power electronics design** (up to 120A, high-voltage 12S LiPo layouts, copper thickness and thermal relief calculation).
*   **Software Development (Current Expert):** C++ / Qt Framework. Cross-platform desktop instrumentation utilities, real-time telemetry plotting, high-precision data logging, and device calibration interfaces.
*   **Peripherals & Interfaces:** Gigabit Ethernet (Microchip switches, LwIP/PHY), CAN bus (including reverse-engineering), UART/USART, SPI, I2C, 1-Wire, Parallel bus (8080), RGB/TFT displays.
*   **FPGA / HDL (Historical / Conceptual Base):** Altera (Intel) MAX II & Cyclone series, Verilog, Intel Quartus Prime. System integration tools (Qsys / Platform Designer / System Building utilities) and peripheral IP cores (UART, etc.). High-speed parallel memory interfacing (SRAM) and video pipelines. *Note: Solid architectural understanding, open to refreshing for specific project needs.*

---

## 📂 FEATURED R&D PROJECTS (Industrial UAV Ecosystem)

### 1. Multi-Processor Industrial Drone Carrier Board (Mission Computer)
*   **Concept:** Designed and built a complex distributed computing and network routing hardware platform for a heavy industrial hexacopter. Managed signal integrity for high-speed communication lines.
*   **Hardware Architecture:** Engineered a multi-layer carrier board featuring:
    *   **STM32F407 (Hardware + Firmware):** Developed custom low-level firmware from scratch to manage real-time communication and flight command injection with the DJI A3 flight controller via native UART API protocols.
    *   **STM32H725V:** Dedicated to high-reliability payload control (winches, searchlights, and peripheral actuators).
    *   **Microchip KSZ9896:** Integrated a 6-port Gigabit Ethernet switch managing internal network routing between a secondary **STM32H7**, an **NVIDIA Jetson Nano** module (hardware integration), and a digital FPV pilot camera.
    *   **Power Delivery Network:** Integrated high-reliability industrial **Mean Well DC-DC converters** to cleanly power all onboard avionics, computer modules, and heavy peripherals.

### 2. High-Power Distribution Board (PDB) & Smart Switch (120A, 12S LiPo)
*   **Concept:** Robust power management system for a heavy industrial drone (25kg MTOW) operating on a high-voltage subsystem to replace bulky mechanical switches with solid-state electronics.
*   **Details:** Designed a high-current PDB capable of handling continuous currents of **100A–120A** under a **12S LiPo (up to 50.4V)** power bus with strict thermal management. Implemented solid-state power switching via high-current MOSFET keys. Developed a companion intelligent control unit driven by an **STM32F103** microcontroller, implementing dedicated **anti-spark protection** and a custom "smart button" power-on sequence (short click followed by a long hold, identical to DJI Phantom sequences) to prevent accidental activation under high voltage.

### 3. Automated UAV Tracking Antenna Gimbal System
*   **Concept:** An Ethernet-controlled Ground Control Station (GCS) directional antenna system that automatically tracks moving UAVs in real-time.
*   **Details:** Engineered an automated pan-tilt gimbal based on an **STM32F407** microcontroller. Routed all power, sensor, and communication lines through mechanical slip rings to allow unlimited 360° continuous rotation. Integrated an onboard GPS, digital compass, and IMU for pitch/roll compensation.
*   **Software:** Developed a custom **C++ / Qt** desktop application that visualizes the antenna’s position on a map, receives telemetry coordinates from the drone in mid-air, and automatically commands the gimbal to follow the UAV's flight path.

### 4. BLDC Motor Test Bench & Custom ESC
*   **Concept:** Diagnostics system for brushless motors to analyze thrust curves and a custom sensorless speed controller.
*   **Details:** Developed a custom Electronic Speed Controller (ESC) from scratch using an **STM32F3** with internal analog comparators, achieving stable sensorless motor startup. Designed a dedicated dyno-test bench utilizing a load cell and a high-precision 24-bit Analog Devices ADC. Wrote a companion **Qt desktop instrumentation app** to plot thrust characteristics in real-time.

### 5. High-Speed Video Processing & Sensors (Historical FPGA Projects)
*   **Details:** Implemented a 25 FPS video capture and display system on an Altera MAX II / Cyclone FPGA, interfacing a 2MP camera, three parallel SRAM chips, and a TFT display with custom freeze-frame buffer logic written in Verilog. Designed a specialized testing rig for reading raw CCD matrix data and streaming it to a PC via UART.

### 6. Digitally Controlled Electronic Load (1000W)
*   **Details:** Designed a high-power digitally managed active load rated for 800W–1000W for laboratory stress-testing and calibration of power delivery networks and batteries.
