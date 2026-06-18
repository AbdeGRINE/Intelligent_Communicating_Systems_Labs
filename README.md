# Intelligent and Communicating Systems (ICS) Labs

## Project Overview

This repository contains a comprehensive series of laboratory projects focused on the design and implementation of microcontroller and single-board computer systems using Arduino and Raspberry Pi platforms. The labs cover everything from basic GPIO manipulation to advanced IoT cloud integration and wired/wireless communication protocols.

---

## Technologies and Hardware

### Microcontrollers & Single-Board Computers
- **Arduino MKR WiFi 1010** — A 32-bit ARM-based board (SAMD21 Cortex-M0+) featuring integrated Wi‑Fi (NINA‑W102) and Bluetooth capabilities.
- **Arduino Uno** — Used for fundamental circuit testing and UART communication experiments.
- **Raspberry Pi 4 Model B** — A microprocessor-based system running Raspberry Pi OS (Linux), used as a full computer for standalone IoT platforms and complex processing.
- **Sonoff Basic R2** — A Wi‑Fi smart switch used for remote AC load control (e.g., LED lamps).

### Sensors & Actuators
- **Light-Dependent Resistor (LDR)** — Measures ambient light intensity for systems like Smart Streetlights.
- **Force-Sensing Resistor (FSR)** — A piezoresistive sensor to detect mechanical pressure/force.
- **Pushbuttons** — For user input with pull‑up/pull‑down resistor configurations and debouncing techniques.
- **LEDs** — Standard and built‑in LEDs for visual output and status indication.
- **ADS1115** — Precision 16‑bit ADC providing analog input capabilities to the Raspberry Pi via I2C.

---

## Protocols & Communication

### Wired Protocols
- **UART (Universal Asynchronous Receiver-Transmitter)** — Point‑to‑point full‑duplex communication between Arduino and Raspberry Pi.
- **I2C (Inter-Integrated Circuit)** — Synchronous bus used to interface the Raspberry Pi with the ADS1115 and other sensors.
- **SPI (Serial Peripheral Interface)** — Explored for high‑speed device interfacing.
- **USB-to-Serial** — Facilitates communication between computers and microcontrollers for debugging and firmware uploads.

### Wireless & Networking
- **Wi‑Fi (802.11 b/g/n)** — Used for network scanning and Internet connectivity.
- **MQTT (Message Queuing Telemetry Transport)** — Lightweight publish/subscribe protocol used for low‑latency data exchange (e.g., with Mosquitto brokers).
- **HTTPS** — Secure communication with cloud‑based IoT services.

---

## Frameworks & Software Tools

### Development Environments
- **Arduino IDE** — Primary tool for authoring and uploading C++ code to Arduino boards.
- **Python** — Main language for Raspberry Pi programming and hardware interfacing; typical libraries include `pyserial`, `RPi.GPIO`, and `adafruit_ads1x15`.

### IoT & Automation Platforms
- **Arduino IoT Cloud** — Real‑time monitoring and control via web dashboards and mobile apps.
- **Blynk** — Create custom mobile interfaces for remote device control.
- **Home Assistant (HassOS)** — Local‑first IoT platform running on Raspberry Pi for privacy and offline operation.
- **Node‑RED** — Flow‑based visual programming tool for wiring hardware devices and APIs, with a real‑time visualization dashboard.
- **eWeLink** — Cloud app used with Sonoff devices for wireless automation.

### Simulation Tools
- **Tinkercad Circuits** — Virtual circuit design and basic Arduino simulation.
- **Proteus** — Advanced schematic capture and microcontroller simulation.

---

## Key Concepts Covered

- **GPIO Management**: Digital I/O and Analog‑to‑Digital Conversion (ADC).
- **PWM (Pulse Width Modulation)**: Simulating analog output for LED brightness or motor speed control.
- **DAC (Digital‑to‑Analog Converter)**: Generating true analog voltages for smooth transitions.
- **Interrupts**: Implementing Interrupt Service Routines (ISRs) for instant event handling (CHANGE, RISING, FALLING).
- **Debouncing**: Solving mechanical signal noise via hardware (RC filters) and software (debounce algorithms/delays).
- **Memory Management**: Monitoring SRAM usage during network operations to ensure device stability.

---

## Getting Started (quick)

1. Open the subdirectory for the lab you want to run (each lab contains hardware lists and step‑by‑step instructions).
2. For Arduino labs: open the `.ino` files in the Arduino IDE and upload to the target board.
3. For Raspberry Pi labs: run Python scripts using `python3`, install dependencies with `pip3 install -r requirements.txt`, and configure I2C/serial as needed.
4. For IoT/cloud labs: follow the README in that lab for required credentials and broker/service setup (e.g., Mosquitto, Arduino IoT Cloud, Blynk).

---

## Contributing

Contributions, improvements, and corrections are welcome. Please open an issue to discuss proposed changes and submit pull requests with clear descriptions and tested code.

---

## License

Specify your preferred license here (e.g., MIT, GPL). If you want, I can add a license file and populate this section.

---

If you'd like, I can also:
- Add per‑lab README entries,
- Create a minimal `requirements.txt` for Raspberry Pi labs,
- Or open a PR to add this README and any additional files — tell me which option you prefer.
