<p align="center">
<img width="693" height="771" alt="1776200614728" src="https://github.com/user-attachments/assets/dab7941f-cd3f-427a-9c80-2718b4669f9c" />

<h1 align="center">4-Layer Wi-Fi Enabled IoT Control Board 🌐</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Project%20Status-Completed-success">
  <img src="https://img.shields.io/badge/Layers-4_Layer_PCB-purple">
  <img src="https://img.shields.io/badge/ECAD-Altium_Designer-blue">
</p>

This repository contains the design and manufacturing files for a 4-layer, Wi-Fi-enabled printed circuit board. The hardware architecture integrates both STM32 and ESP32 microcontrollers, designed specifically for robust IoT applications. The system features direct 220V AC mains power handling and multiple environmental sensor interfaces, strictly adhering to Design for Manufacturing (DFM) principles.

## 🛠️ Technical Highlights

* 🧠 **Dual Microcontroller Architecture**
    Combines the real-time processing capabilities of an STM32 microcontroller with an ESP32 module to manage Wi-Fi communication and network connectivity operations simultaneously.
* ⚡ **High-Voltage Power Integration**
    Features an onboard power supply section capable of safely and efficiently regulating a 220V AC input down to the required DC logic levels (+5V, +3.3V).
* 📡 **Sensor Array Integration**
    Includes dedicated hardware routing and interfaces for external environment monitoring, specifically integrating PIR (motion) and temperature sensors.
* 🔀 **Multi-Protocol Communication**
    The hardware layout incorporates standard embedded communication protocols, providing dedicated traces for UART, SPI, and I2C to allow modular peripheral expansion.
* 🏭 **Industrial DFM Standards**
    Utilizes a 4-layer PCB stackup to ensure proper signal integrity, optimized power distribution, and EMI reduction, ready for industrial fabrication.

## ⚙️ Technical Specifications

<div align="center">

| System Parameter | Specifications |
| :--- | :--- |
| **PCB Layer Count** | 4 Layers |
| **Primary MCUs** | STM32 & ESP32 |
| **Power Input** | 220V AC Mains |
| **Communication Protocols** | UART, SPI, I2C, Wi-Fi |
| **Integrated Sensors** | PIR (Motion), Temperature |

---
*Acknowledgments: This board was designed and routed as the capstone project for the "PCB Design - Life Cycle of an Electronic Card" training program by xBowtie Turkey, instructed by Mustafa Berk AYDOĞAN.*
