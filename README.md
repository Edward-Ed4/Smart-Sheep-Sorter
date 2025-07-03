# 🐑 Automated Smart Sheep Sorter

An embedded system that automatically identifies and sorts sheep based on wool presence using ESP32-CAM and Arduino Uno.

## 📋 Project Overview

This system captures an image of each sheep using an ESP32-CAM and classifies them based on visible wool coverage. The result is sent to an Arduino Uno, which controls servo motors to direct sheep into separate pens and updates an LCD with status and count.

| Technology       | Component               |
|------------------|--------------------------|
| Microcontroller  | ESP32-CAM, Arduino Uno |
| Actuators        | 2× SG90 Servo Motors     |
| Display          | 16×2 I2C LCD             |
| Power Supply     | 5V/2A                    |
| Programming      | Arduino IDE, C++         |

## 🎯 Features

- 🧠 Image-based wool detection
- 🔀 Servo-actuated automatic sorting gates
- 📺 LCD display for real-time feedback
- 💬 Serial communication between ESP32 and Arduino

## 📂 Project Structure

```
├── ESP32-CAM/
│   └── main_camera_code.ino
├── Arduino/
│   └── gate_controller.ino
├── docs/
│   └── report.pdf
│   └── poster.png
├── images/
│   └── system_diagram.png
└── README.md
```

## 🚀 Getting Started

### 🧰 Requirements

- ESP32-CAM module
- Arduino Nano + USB cable
- 2x SG90 Servos
- 16x2 I2C LCD
- Breadboard + jumper wires
- Power supply (5V, 2A)

### 🧪 Setup

1. Flash the ESP32-CAM code using an FTDI adapter.
2. Upload Arduino code for servo and LCD control.
3. Wire components:
   - ESP32 to FTDI
   - Arduino to LCD and servos
4. Power up and test classification → gate direction → LCD update.

## 📷 Demo

![System Architecture](images/system_diagram.png)

## 📊 Work Plan

| Week | Tasks                            |
|------|----------------------------------|
| 1    | Design + Component Setup         |
| 2    | Code Development + Wiring        |
| 3    | Integration + Testing + Report   |

## 👥 Team Members

- **Ssenyange Allan** – Poster & testing
- **Omara Emmanuel** – Website & ESP32 UART
- **Kimera Dave David** – Architecture & chute
- **Ebaju Edward** – Report & ML logic
- **Nabasirye Seanice** – Equipment & LCD wiring

## 📜 License

MIT License

---

## 📎 Helpful Links

- [ESP32-CAM Docs](https://randomnerdtutorials.com/esp32-cam-video-streaming-web-server-camera-home-surveillance/)
- [Servo Arduino Guide](https://www.arduino.cc/en/Reference/Servo)
- [LCD I2C Setup](https://randomnerdtutorials.com/arduino-display-on-lcd-i2c/)
