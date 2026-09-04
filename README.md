# 🤖 ESP32-C3 Smart Robot Car

A DIY 2WD robot car built using an **ESP32-C3**, **L298N dual H-bridge motor driver**, **DC gear motors**, and an **OLED display**.

The robot features a handmade copper-wire chassis and was programmed using the **Arduino IDE**.

---

## 📸 Project Photos

### Front View
![Robot Front](images/robot-front.jpg)

### Rear View
![Robot Rear](images/robot-back.jpg)

### Top View
![Robot Top](images/robot-top.jpg)

---

## ✨ Features

- ESP32-C3 based control system
- 2-wheel drive
- Two DC geared motors
- L298N dual H-bridge motor driver
- OLED display
- USB Type-C charging
- Rechargeable battery
- Handmade copper-wire chassis
- LED lighting
- Arduino IDE programmable

---

## 🛠️ Components

| Component | Quantity |
|---|---:|
| ESP32-C3 | 1 |
| DC Gear Motors | 2 |
| L298N 2-Way Dual H-Bridge DC Driver | 1 |
| OLED Display | 1 |
| Type-C Charging Module | 1 |
| Battery | 1 |
| Wheels | 2 |
| Switch | 1 |
| 1 mm Copper Wire | As required |
| 0.8 mm Copper Wire | As required |

---

## 🔌 Wiring / Connections

### ESP32-C3 → L298N

| ESP32-C3 | L298N |
|---|---|
| GPIO ___ | IN1 |
| GPIO ___ | IN2 |
| GPIO ___ | IN3 |
| GPIO ___ | IN4 |
| GND | GND |

### L298N → DC Motors

| L298N | Motor |
|---|---|
| OUT1 | Left Motor |
| OUT2 | Left Motor |
| OUT3 | Right Motor |
| OUT4 | Right Motor |

### OLED → ESP32-C3

| OLED | ESP32-C3 |
|---|---|
| VCC | 3.3V |
| GND | GND |
| SDA | GPIO ___ |
| SCL | GPIO ___ |

> Replace the GPIO numbers with the actual pins used in the project.

### Power Connections

The rechargeable battery is connected to the power system through the **Type-C charging module** and **power switch**.

The L298N controls and powers the two DC gear motors.

---

## 💻 Software / Libraries

### Software

- **Arduino IDE**
- **C/C++**
- ESP32 board support package

### Libraries

Depending on the OLED code, the following libraries may be required:

```text
Wire
Adafruit GFX
Adafruit SSD1306
