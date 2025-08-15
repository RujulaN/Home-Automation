# 🏠 Home Automation with Arduino IoT Cloud using ESP32

## 📌 Project Overview
This project implements a **smart home automation system** using an **ESP32** microcontroller and the **Arduino IoT Cloud**.  
It enables **remote monitoring and control** of home appliances, ensuring security, safety, and energy efficiency.

---

## ✨ Features

### 1️⃣ RFID-based Door Security
- Grants access only to authorized RFID tags.
- Unauthorized access triggers a buzzer alarm.

### 2️⃣ Automatic Water Tank Management
- Monitors water levels using sensors.
- Automatically starts the pump when the tank is empty and stops it when full.

### 3️⃣ LPG Gas Leak Detection & Safety System
- Detects gas leakage in the kitchen.
- Automatically:
  - Cuts off kitchen power supply
  - Closes gas regulator
  - Activates buzzer alarm
  - Turns on exhaust fan
- Sends alerts via IoT Cloud.

### 4️⃣ Automatic Lighting System
- Detects ambient light and human presence.
- Turns lights on in darkness and off when not needed.
- Saves energy efficiently.

---

## 🛠 Components Used
- **ESP32 Development Board**
- **RFID Module (RC522)**
- **Water Level Sensor**
- **Gas Sensor (MQ-2 / MQ-5)**
- **PIR Motion Sensor**
- **LDR Sensor**
- **Relay Module**
- **Buzzer**
- **Arduino IoT Cloud** platform
- Jumper wires, breadboard, and power supply

---

## 🔌 Working Principle
1. **Sensors** continuously monitor environmental conditions (water level, gas, light, motion).
2. **ESP32** processes sensor data and sends it to the **Arduino IoT Cloud**.
3. **User Interface**: Mobile app or web dashboard for remote control and monitoring.
4. **Automation Rules**: Based on sensor readings, devices are switched on/off automatically.

---

