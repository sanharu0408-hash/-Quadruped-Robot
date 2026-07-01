# 🐾 Quadruped Robot Project

This project features a 4-legged walking robot controlled via an Arduino R4 and a Python-based PC controller.

## 📁 Project Structure

- `/controller`: Python source code for PC-side control (Pygame & Serial).
- `/arduino_code`: Arduino sketch for servo motor management (PCA9685).
- `/STL`: 3D printable parts for the robot chassis.

## 🖨️ 3D Printing Guide

Please print the following components from the `/STL` folder. 
The recommended material is PLA or PETG with at least 20% infill for durability.

| File Name | Quantity | Description |
|:---|:---:|:---|
| `frame_bottom.stl` | 1 | Main lower chassis |
| `frame_top.stl` | 1 | Upper cover / battery holder |
| `hip_1.stl` | 2 | Inner hip joints |
| `hip_2.stl` | 2 | Outer hip joints |
| `left_knee.stl` | 2 | Knee parts for Left side |
| `right_knee.stl` | 2 | Knee parts for Right side |

*Note: In the screenshot, `frame_top` was labeled as `frame_tom`. Please rename it for consistency.*

## 🚀 Getting Started

### 1. Arduino Setup
1. Open `arduino_code/arduino_code.ino` in the Arduino IDE.
2. Install the `Adafruit PWM Servo Driver` library.
3. Upload the code to your Arduino R4.

### 2. Python Controller Setup
1. Install the required libraries:
   ```bash
   pip install pygame pyserial
