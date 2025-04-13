# Smart_Parking_System
# 🚗 IoT-Based Car Parking System

An automated smart parking system designed using **Arduino Uno**, **IR sensors**, **a servo motor**, and an **I2C LCD display**. This project helps efficiently manage limited parking spaces by detecting vehicle entry and exit, updating availability in real time, and controlling access through a motorized gate.

---

## 📌 Features

- ✅ Real-time vehicle detection using **IR sensors**
- ✅ Parking space tracking and availability management
- ✅ Automated gate control via **servo motor**
- ✅ Live parking status displayed on **16x2 I2C LCD**
- ✅ Simple and cost-effective system for smart parking

---

## 🧰 Hardware Requirements

| Component           | Quantity |
|---------------------|----------|
| Arduino Uno         | 1        |
| IR Sensor Module    | 2        |
| Servo Motor (SG90)  | 1        |
| 16x2 I2C LCD        | 1        |
| Jumper Wires        | As needed |
| Breadboard          | 1        |
| Power Supply        | 1        |

---

## 🔌 Circuit Connections

| Component      | Arduino Pin |
|----------------|-------------|
| IR Sensor 1    | D2          |
| IR Sensor 2    | D3          |
| Servo Motor    | D9          |
| I2C LCD        | SDA → A4, SCL → A5 |

> ⚠️ **Note:** Power the servo through an external 5V source if the USB port can't provide enough current.

---

## 🧠 How It Works

1. **IR Sensor 1** detects a car at the **entry gate**.
   - If space is available:
     - Servo gate opens.
     - Available space count is reduced by 1.
   - If no space is available:
     - "No Space Available" is displayed on the LCD.

2. **IR Sensor 2** detects a car at the **exit**.
   - Servo gate opens.
   - Available space count increases by 1.

3. **16x2 LCD** displays:
   - Total parking slots
   - Currently available slots

---



