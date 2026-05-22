<p align="center">
<img width="340" height="561" alt="Screenshot 2026-05-22 150440" src="https://github.com/user-attachments/assets/2a7a63c5-e329-4f31-8f82-f80aaa692749" />

<h1 align="center">Breadboard Power Supply Module ⚡</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Project%20Status-Completed-success">
  <img src="https://img.shields.io/badge/ECAD-KiCad-blue">
</p>

## 🛠️ Technical Highlights

* 🔌 **Master Power Control**
    Utilizes a barrel jack connector for the primary DC input (e.g., +12V). It features an integrated master slide switch for direct, hardware-level on/off control of the entire circuit.
* ⚡ **Dual Voltage Regulation**
    Employs an LM7805 linear regulator for the +5V rail and an LM317 adjustable regulator (configured via a resistor divider) for the +3.3V rail. Both rails are stabilized with bypass capacitors.
* 🔀 **Independent Output Routing**
    Dual 3-pin jumper headers allow the user to independently route either +5V or +3.3V to the top and bottom breadboard rails without requiring structural modifications.
* 🔗 **Auxiliary Terminals**
    Includes onboard screw terminals to securely power external sensors or peripheral modules directly from the main PCB.

> **System Benefit:** This module eliminates the need for multiple external power supplies, ensuring precise and safe voltage management for mixed-signal embedded systems.

## ⚙️ Technical Specifications

<div align="center">

| Feature / Component | Details / Specifications |
| :--- | :--- |
| **Primary Input** | DC Barrel Jack (Optimal: +7V to +12V) |
| **+5V Regulation** | LM7805 Linear Voltage Regulator |
| **+3.3V Regulation** | LM317 Adjustable Regulator (Divider Configured) |
| **Breadboard Routing** | Dual 3-Pin Headers (J3, J4) |
| **Auxiliary Output** | Onboard Screw Terminals (J5, J7) |
| **Status Indicator** | Power-ON Red LED (D1) |

</div>

---
*Note: This project was developed based on the hardware design principles taught in Dr. Peter Dalmaris's Udemy course.*
