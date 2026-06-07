# Engineering Portfolio: Mike Miller

Welcome to my portfolio! I am a Hardware Design Engineer focused on wearable sensor integration, embedded systems, and PCB design. This page showcases my R&D process, design methodology, and debug logs.

---

## 🛠 Skills & Competencies
* **PCB Design:** KiCad (Schematic Capture, Layout, DFM)
* **Embedded Systems:** nRF5340, STM32WB, BLE Firmware integration
* **Analog/Mixed Signal:** ECG/EMG AFE designs, Audio/Optical systems
* **Instrumentation:** Oscilloscopes, Multimeters, Logic Analyzers

---

## 🚀 Featured Projects

### 1. Wireless EMG Wearable
*A compact, low-power wearable device for EMG signal acquisition.*

#### Overview
- **Objective:** Design a small-scale wearable EMG sensor node with integrated BLE for remote monitoring.
- **Key Components:** STM32 MCU, Custom Analog Front End (AFE), LiPo Battery.

#### Engineering Process
- **Design Philosophy:** Focused on miniaturization and high SNR for biosignals.
- **CAD/Layout:** ![Top](C:\Users\mmill\OneDrive\Documents\GITPAGE\EMG1_TOP.png) ![Bottom] (C:\Users\mmill\OneDrive\Documents\GITPAGE\EMG1_BOTTOM.png)
- **Debug Log / Lessons Learned:**
    - **Issue:** Encountered a short on the SWDCLK line during bring-up.
    - **Root Cause:** Inadequate via-to-pour clearance in the initial layout.
    - **Resolution:** Validated via continuity testing.
    - **Future Iteration:** Increased clearance rules in Altium to prevent shorts in Rev B.

#### Status
- **Current Phase:** Architecture validated. Analog AFE performance verified; digital core transitioning to modular "Core/Carrier" architecture for Rev B.

---

## 🔍 Current R&D: "Golden Reference" Platform
I am currently developing a modular "Golden Reference" motherboard for the nRF5340. 
* **Goal:** To decouple digital bring-up from complex sensor/analog integration.
* **Architecture:** Core board (MCU/Power) + Carrier board (AFEs/Sensors).
* **Expected Outcome:** A proven baseline for all future wearable sensor iterations.

---

## 📧 Contact
- **LinkedIn:** [Insert Link]
- **Email:** [Insert Email]
