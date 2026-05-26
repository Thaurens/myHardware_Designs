<p align="center">
<img width="1712" height="896" alt="Tiny_Solar_Power_Supply" src="https://github.com/user-attachments/assets/521928d5-c2dd-4bf3-87de-3e529452a68b" />

# ☀️ Tiny Solar Power Supply (1.2V to 3.3V Auto-Switching)

This repository contains the hardware design files for a Tiny Solar Power Supply. **I have completed the design of this module, developed as part of Peter Dalmaris' hardware design course on Udemy.** The goal of this project is to repurpose standard solar garden light components (a mini solar panel and a 1.2V Ni-MH rechargeable battery) into a reliable power source for small electronics. Unlike standard garden lights that provide an unregulated voltage, this module outputs a clean, regulated 3.3V, making it ideal for powering low-power microcontrollers and IoT sensors.

## 📌 Project Overview
The core of the design is the **AP3015 DC-DC Boost Converter**, which efficiently steps up the 1.2V battery voltage to 3.3V. To conserve energy, the circuit features an autonomous switching mechanism that detects ambient light conditions entirely through hardware.

## ✨ Key Features
* **Input:** 1.2V Ni-MH Rechargeable Battery (AA/AAA) & Mini Solar Panel.
* **Output:** Regulated 3.3V DC.
* **Hardware Auto-Sleep/Wake:**
  * ☀️ **Day Mode (Charging):** The solar panel charges the battery. The panel voltage drives the gate of a 2N7002 MOSFET, pulling the `SHDN` (Shutdown) pin of the AP3015 to ground. The regulator sleeps, and the 3.3V output is disabled.
  * 🌙 **Night Mode (Discharging):** When the panel voltage drops in the dark, the MOSFET turns off. The AP3015 wakes up and begins boosting the battery voltage to 3.3V.

## 🛠️ Working Principle & Topology
The circuit can be divided into three main stages:
1. **Charging Stage:** Energy from the solar panel flows through a Schottky diode (SS14) into the battery, preventing reverse leakage at night.
2. **Switching Stage:** The Q1 MOSFET acts as a light-dependent switch. It toggles the regulator's shutdown pin based on the presence of solar voltage.
3. **Boost Stage:** The U1 IC (AP3015) drives an inductor (L1, 10uH). The resulting flyback voltage is rectified by D1 and smoothed by C2. The feedback voltage divider (R1 and R2) strictly maintains the output at 3.3V.
