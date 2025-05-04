# ChemAgent: Smart Chemical Dispensing System

**ChemAgent** is an Arduino-based chemical dispensing machine designed for educational and research chemistry labs. Controlled via a custom-built Bluetooth mobile app, it allows users to select individual chemicals or compounds and dispense them in precise milliliter (ml) quantities — reducing manual handling and ensuring accuracy and safety.

---

## Features

- 📲 **Bluetooth Control** via a dedicated mobile app  
- 🧪 **Individual Chemical Dispensing** (e.g., Sulfur, Oxygen)  
- ⚗️ **Compound Creation Logic** (e.g., H₂SO₄ from S and O)  
- 💧 **Precision Dosing** using calibrated water pumps  
- 🧠 **Automated Mixing** of common reagents  
- 💡 **Easy-to-use Interface** for students and lab assistants

---

## Hardware Components

| Component            | Description                    |
|----------------------|--------------------------------|
| Arduino UNO          | Main controller                |
| Bluetooth Module HC-05 | Wireless communication with mobile app |
| Water Pump(s)        | Dispenses selected liquids     |
| Power Supply         | Powers the system              |
| Relay Module         | Controls pumps safely          |
| Tubing System        | For chemical flow              |

---

## Mobile App Overview

- Connects via Bluetooth to Arduino
- User selects:
  - **Chemical Name**
  - **Desired Quantity (in ml)**
- App sends formatted command to Arduino
- Includes preset options like:
  - `H₂SO₄` → automatically dispenses correct S and O quantities

---

## Arduino Code

The Arduino sketch:
- Parses incoming Bluetooth data
- Activates corresponding pumps
- Supports both **individual chemicals** and **compound mixing logic**

