# 🧭 DP WiFi Transceiver [Project ID: P-34]

A MATLAB App Designer and Simulink–based WiFi transceiver (TRX) application for configuring, simulating, and working with DP WiFi systems using MCS 13 and related signal-processing models.

---

## 📚 Table of Contents

[About](#-about)  
[Features](#-features)  
[Tech Stack](#-tech-stack)  
[Installation](#️-installation)  
[Usage](#-usage)  
[Configuration](#-configuration)  
[Screenshots](#-screenshots)  
[Project Structure](#-project-structure)  
[Contact](#-contact)  
[Acknowledgements](#-acknowledgements)

---

## 🧩 About

This project provides a desktop application for DP WiFi transceiver design and simulation. It combines an intuitive **MATLAB App Designer** GUI with **Simulink** models so you can configure parameters, run simulations, and analyze WiFi PHY behavior (including MCS 13 and DP32-style configurations) without writing scripts from scratch.

**Key goals:**

- Offer a single entry point (the app) to run and control transceiver simulations.
- Support parameter-driven experiments via the GUI and linked Simulink models.
- Package the solution for distribution (e.g., as an installable app with uninstaller).

---

## ✨ Features

- **Graphical control** – Configure and run transceiver simulations from the DPWiFi_TRX app.
- **Simulink models** – Encoder, receiver, time-sync, and MCS13/DP32 WiFi PHY models (B, E, R, TS, MCS13WiFi_DP32).
- **Packaged deployment** – Installable application with icon and uninstaller (Uninstal.exe).
- **Modular design** – Separate .slx models for encoding (E), reception (R), time sync (TS), and main MCS13 WiFi chain (MCS13WiFi_DP32) for easier maintenance and reuse.

---

## 🧠 Tech Stack

| Category   | Technologies |
|-----------|--------------|
| **Languages** | MATLAB (App Designer, scripts) |
| **Frameworks** | MATLAB App Designer, Simulink |
| **Models** | Simulink (.slx): B, E, R, TS, MCS13WiFi_DP32 |
| **Tools** | MATLAB, Simulink (and toolboxes as required by the models) |

---

## ⚙️ Installation

1. **Prerequisites:** MATLAB (and Simulink) installed, with any toolboxes required by the Simulink models (e.g., Communications Toolbox, DSP System Toolbox—depending on block usage).

2. **Option A – From source (project folder)**  
   - Clone or copy the project folder to your machine.  
   - Open MATLAB and set the project folder as the current directory (or add it to the MATLAB path).  
   - Open the app: in the **Apps** tab, use **Open** and select `DPWiFi_TRX.mlapp`, or run:

## 🚀 Usage

1. **Start the app**  
   - In MATLAB: open `DPWiFi_TRX.mlapp` from the Apps gallery or run `DPWiFi_TRX` from the command window.  
   - If using a packaged install: launch the “DP WiFi Transceiver” (or equivalent) shortcut from the Start Menu or desktop.

2. **Run simulations**  
   - Set parameters in the app (carrier, MCS, gains, etc., as exposed by the GUI).  
   - Use the app controls to start simulations that invoke the Simulink models (e.g., MCS13WiFi_DP32, E, R, TS).  
   - View results in the app (plots, status, logs) or in Simulink scopes/data exported to the workspace.

3. **Work with models directly (optional)**  
   - Open `Simulink/*.slx` in Simulink to inspect or modify the block diagrams.  
   - Run individual models from Simulink or call them from the app/scripts as designed.

---

## 🧾 Configuration

- **MATLAB path:** Ensure the project root (and optionally `Simulink/`) is on the MATLAB path so the app and models load correctly.  
- **Simulink models:** Paths or model names referenced inside the app must match the actual `.slx` files in the `Simulink/` folder.  
- **Toolboxes:** Confirm required toolboxes (e.g., Communications, DSP, RF) are installed if you see missing-block or license errors when opening the app or models.

No `.env` file is used; configuration is through the app UI and/or Simulink model parameters.

---

## 🖼 Screenshots


## 📬 Contact

**Author:** Jeremy Gomez  
**Email:** jeremygz0607@gmail.com  
**GitHub:** @jeremygz0607  

---

## 🌟 Acknowledgements

- MathWorks MATLAB and Simulink documentation.  
- Communications / DSP toolboxes and block libraries used in the Simulink models.  
- Icons and assets (e.g., icon.ico) as per your project sources.  
