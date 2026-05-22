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

---
*Note: This project was developed based on the hardware design principles taught in Dr. Peter Dalmaris's Udemy course.*
