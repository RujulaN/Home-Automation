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

## 🛠 Components and Their Working

### **1. ESP32 Microcontroller**
- **Purpose:** The brain of the system.
- **Working:**
  - Reads data from sensors (RFID, gas sensor, LDR, PIR, water level sensor).
  - Controls actuators (relay, buzzer, exhaust fan, lights).
  - Connects to **Arduino IoT Cloud** via Wi-Fi for remote monitoring and control.

### **2. RFID Module (RC522)**
- **Purpose:** Provides secure door access.
- **Working:**
  - Reads the unique ID of an RFID tag.
  - If the ID matches a stored authorized ID, the ESP32 unlocks the door.
  - Unauthorized attempts trigger the buzzer.

### **3. Water Level Sensor**
- **Purpose:** Monitors water tank levels.
- **Working:**
  - Detects water presence at different levels.
  - Empty tank → motor ON.
  - Full tank → motor OFF.

### **4. Gas Sensor (MQ-2 / MQ-5)**
- **Purpose:** Detects LPG gas leaks.
- **Working:**
  - Monitors air for LPG concentration.
  - On leak detection → cuts kitchen power, closes regulator, activates buzzer, turns on exhaust fan, and sends IoT alert.

### **5. PIR Motion Sensor**
- **Purpose:** Detects human movement.
- **Working:**
  - Senses infrared changes caused by movement.
  - In darkness, motion triggers lights ON.

### **6. LDR (Light Dependent Resistor)**
- **Purpose:** Detects light intensity.
- **Working:**
  - Low light → triggers lights ON (if motion detected).
  - Bright light → lights OFF.

### **7. Relay Module**
- **Purpose:** Controls high-voltage devices.
- **Working:**
  - Acts as a switch controlled by ESP32 to turn appliances ON/OFF.

### **8. Buzzer**
- **Purpose:** Gives audible alerts.
- **Working:**
  - Activated during unauthorized access or emergencies.

### **9. Arduino IoT Cloud**
- **Purpose:** Enables remote access.
- **Working:**
  - Receives real-time data from ESP32.
  - Allows monitoring and control via web or mobile dashboard.



