# Flame Detector
An Arduino Uno-based flame detection system using an IR flame sensor and an OLED display to detect flames and display real-time safety alerts.
# 🔥 IR Flame Detector Using Arduino Uno and OLED

## 📌 Project Overview
This project is a simple flame detection system built using an Arduino Uno, an infrared (IR) flame sensor, and an I²C OLED display. The system detects infrared radiation associated with a flame and displays the detection status in real time.

When a flame is detected, the OLED displays a warning message. Otherwise, it displays a safe status.

## ✨ Features
- Real-time flame detection using an IR flame sensor.
- OLED display for clear status messages.
- Arduino Serial Monitor output for debugging.
- Simple, low-cost hardware implementation.
- Expandable for future fire-alert projects.

## 🧰 Components Required
| Component | Quantity |
|---|---:|
| Arduino Uno | 1 |
| IR Flame Sensor Module | 1 |
| SSD1306 I²C OLED Display (128×64) | 1 |
| Jumper Wires | As required |
| USB Cable | 1 |

## 🔌 Circuit Connections

| Component | Pin | Arduino Uno |
|---|---|---|
| Flame Sensor | VCC | 5V |
| Flame Sensor | GND | GND |
| Flame Sensor | DO | Digital Pin 2 |
| OLED | VCC | According to module rating |
| OLED | GND | GND |
| OLED | SDA | A4 |
| OLED | SCL | A5 |

**Note:** Verify the OLED module's voltage requirements before powering it.

## 💻 Software Requirements
- Arduino IDE
- Adafruit GFX Library
- Adafruit SSD1306 Library
- Wire Library (included with Arduino IDE)

## ⚙️ Working Principle
1. The IR flame sensor detects infrared radiation from a flame.
2. The sensor's digital output is read by Arduino Uno.
3. The Arduino processes the sensor state.
4. The OLED displays either `FLAME DETECTED` or `SAFE`.
5. The Serial Monitor displays the current detection status.

The example code assumes that the sensor output goes LOW when a flame is detected. Sensor modules may behave differently, so verify the output before use.

## 🚀 How to Run
1. Connect the components according to the wiring table.
2. Install the required Arduino libraries.
3. Open the Arduino sketch in Arduino IDE.
4. Select **Arduino Uno** under Tools → Board.
5. Select the correct COM port.
6. Upload the code.
7. Observe the OLED display and Serial Monitor.

## 🔮 Future Improvements
- Add a buzzer for audible alerts.
- Add an LED warning indicator.
- Integrate temperature and smoke sensors.
- Send alerts using an ESP32 and Wi-Fi.
- Add event logging and a fire-alert notification system.

## ⚠️ Safety Disclaimer
This project is intended for educational and experimental purposes. An inexpensive IR flame sensor can produce false readings and cannot reliably detect every fire condition. This prototype is not a substitute for a certified fire detection or alarm system.

## 📜 License
This project may be distributed under the MIT License if the repository owner chooses to apply it.
