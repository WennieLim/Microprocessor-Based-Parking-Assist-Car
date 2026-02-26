# Microprocessor-Based Parking Assist Car

# Project Overview
This project implements a microprocessor-based parking assist system using STM32 and multiple sensors to help a vehicle align correctly within a parking space and detect nearby obstacles.

The system provides:
- Visual indication using LEDs for alignment status
- Audio warning using a buzzer when an obstacle is detected

---

# Hardware Components
- STM32 Microcontroller
- IR Sensors ×4 (Parking alignment detection)
- KY-032 Obstacle Avoidance Sensor
- Yellow LED – Correct parking position indicator
- Red LED – Incorrect position indicator
- Buzzer – Obstacle alert

---

# Pin Configuration

| Pin | Function |
|-----|----------|
| PA0 | Yellow LED |
| PA1 – PA4 | IR Sensors |
| PA5 | KY-032 Obstacle Sensor |
| PA6 | Buzzer |
| PA7 | Red LED |

---

# System Operation

# Parking Alignment Detection
- All IR sensors detect the correct region → Yellow LED ON
- Any IR sensor not aligned → Red LED ON

# Obstacle Detection
- Obstacle detected by KY-032 → Buzzer ON
- No obstacle → Buzzer OFF

---

# Software Description
The system is developed using **STM32 HAL**.

Main processes:
1. GPIO initialization for sensors, LEDs, and buzzer
2. Continuous reading of IR sensors
3. Alignment status evaluation
4. Obstacle detection monitoring
5. Output control for LEDs and buzzer

---

# Initialization
A short delay is added during startup to allow sensor stabilization.

---

# Development Environment
- STM32CubeIDE
- Embedded C
- STM32 HAL Driver

---

# Demonstration
https://www.youtube.com/watch?v=z2rG7ZfbP-E 

---

# Author
**Wennie Lim**  
Electronic Engineering Student  
Universiti Teknologi Malaysia
