# 📡 Arduino Ultrasonic Radar

<p align="center">
  <b>Real-Time Object Detection & Radar Visualization</b>
  <br>
  An embedded systems project combining ultrasonic sensing, servo motor control, and real-time data visualization.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Arduino-Uno_R3-00979D?style=for-the-badge&logo=arduino&logoColor=white" />
  <img src="https://img.shields.io/badge/Language-C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/Visualization-Processing-006699?style=for-the-badge" />
</p>

---

## 🚀 Overview

The **Arduino Ultrasonic Radar** is a real-time object detection system built using an Arduino Uno R3, an HC-SR04 ultrasonic sensor, and an SG90 servo motor.

The ultrasonic sensor measures the distance to nearby objects while the servo motor continuously rotates the sensor across a 150° scanning range. Distance and angular measurements are transmitted to a computer through serial communication and visualized using **Processing**, creating a radar-style interface that displays detected objects in real time.

## ✨ Features

- 📡 **Ultrasonic Detection:** Measures distances to nearby objects using the HC-SR04 sensor.
- 🔄 **Automated Scanning:** Servo motor provides continuous 15°–165° scanning.
- 📏 **Distance Measurement:** Calculates object distances using ultrasonic pulse timing.
- 📊 **Real-Time Visualization:** Displays sensor readings through a Processing-based radar interface.
- 🔌 **Serial Communication:** Transmits angular and distance measurements between Arduino and computer.
- 🔊 **Proximity Alert:** Optional buzzer feedback when objects are detected within a defined range.

## 🛠️ Hardware Components

| Component | Purpose |
|:---|:---|
| Arduino Uno R3 | Main microcontroller |
| HC-SR04 Ultrasonic Sensor | Object detection and distance measurement |
| SG90 Servo Motor | Rotates the ultrasonic sensor |
| Breadboard | Circuit assembly |
| Jumper Wires | Electrical connections |
| Buzzer | Optional proximity alert |

## 💻 Software & Technologies

- **C++** – Embedded programming and hardware control
- **Arduino IDE 2.x** – Code development and microcontroller programming
- **Processing 4.x** – Radar visualization and graphical interface
- **Serial Communication** – Real-time data transmission
- **Arduino Servo Library** – Servo motor control

## 🔌 Circuit & Pin Configuration

| Component | Arduino Connection |
|:---|:---|
| HC-SR04 VCC | 5V |
| HC-SR04 GND | GND |
| HC-SR04 TRIG | Digital Pin 10 |
| HC-SR04 ECHO | Digital Pin 11 |
| SG90 Signal | Digital Pin 12 |
| SG90 VCC | 5V |
| SG90 GND | GND |
| Buzzer (Optional) | Analog Pin A0 |

## 📂 Project Structure

```text
Arduino-Ultrasonic-Radar/
│
├── Arduino/
│   └── UltrasonicRadar.ino
│
├── Processing/
│   └── ArduinoRadar.pde
│
├── Images/
│   └── radar-demo.jpg
│
└── README.md
```

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Arduino-Ultrasonic-Radar.git
cd Arduino-Ultrasonic-Radar
```

### 2. Set Up the Arduino

1. Open `Arduino/UltrasonicRadar.ino` in Arduino IDE.
2. Connect the Arduino Uno to your computer.
3. Select **Arduino Uno R3** as the target board.
4. Select the appropriate serial port.
5. Upload the sketch.

### 3. Configure Processing

1. Install [Processing](https://processing.org/download).
2. Open `Processing/ArduinoRadar.pde`.
3. Configure the serial port to match your connected Arduino.
4. Ensure the baud rate is set to `9600`.
5. Run the Processing sketch.

> **Note:** Close the Arduino Serial Monitor before launching Processing, as both applications cannot access the same serial port simultaneously.

### 4. Run the Radar

Once both programs are running, the servo motor will continuously scan its surroundings while the Processing interface displays:

- 🟢 Radar scanning beam
- 🔴 Detected objects
- 📐 Current scanning angle
- 📏 Measured object distance

## 🧠 Engineering Concepts

This project explores several fundamental concepts in automation and embedded systems:

- **Embedded Systems:** Programming microcontrollers to interact with physical hardware.
- **Sensor Integration:** Interfacing with ultrasonic sensors to acquire environmental data.
- **Actuator Control:** Implementing servo motor positioning and automated scanning.
- **Signal Processing:** Converting ultrasonic pulse duration into distance measurements.
- **Serial Communication:** Transmitting sensor data between embedded hardware and a computer.
- **Real-Time Visualization:** Transforming raw sensor measurements into an interactive graphical representation.

## 🔮 Future Improvements

- [ ] Implement object tracking across multiple scans.
- [ ] Improve distance measurement accuracy and filtering.
- [ ] Add configurable scanning angles and rotation speeds.
- [ ] Develop an enhanced radar interface.
- [ ] Introduce wireless data transmission.
- [ ] Expand detection capabilities and proximity alerts.

<p align="center">
  <i>Exploring the intersection of embedded systems, electronics, and intelligent automation.</i>
</p>

## Demo

<img width="534" height="540" alt="Screenshot 2026-11-22 at 10 21 43 PM" src="https://github.com/user-attachments/assets/404713e6-745a-4eca-bc3b-55cac2ad730e" />

