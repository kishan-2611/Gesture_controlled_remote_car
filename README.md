# Gesture Controlled Remote Car

## Overview

The Gesture Controlled Remote Car is an embedded systems project designed using **ATmega16**, **MPU6050 IMU sensor**, **HC-05 Bluetooth module**, and **L293D motor driver**. The system enables real-time vehicle movement based on hand gestures by detecting motion through the MPU6050 accelerometer and gyroscope.

The transmitter unit captures hand tilt and movement using the MPU6050 sensor, processes the data through the ATmega16 microcontroller, and sends directional commands wirelessly via the HC-05 Bluetooth module. The receiver unit receives these commands and controls the 4WD robotic car motors using the L293D motor driver.

This project demonstrates practical implementation of:
- Embedded C Programming
- Bare-metal Firmware Development
- I2C Communication (MPU6050)
- UART Communication (HC-05 Bluetooth)
- Wireless Control Systems
- Real-time Motor Driver Control

---

## Features

- Real-time gesture-based movement control
- Wireless Bluetooth communication
- Low-latency response system
- Forward, Backward, Left, Right movement control
- 4WD motor drive support
- MPU6050 accelerometer + gyroscope integration
- Embedded C bare-metal programming

---

## Hardware Components Used

- ATmega16 Microcontroller
- MPU6050 Accelerometer + Gyroscope Sensor
- HC-05 Bluetooth Module
- L293D Motor Driver IC
- 4 DC Motors
- 4WD Robot Chassis
- Battery Pack
- Voltage Regulator
- Connecting Wires

---

## Working Principle

### Transmitter Side

1. MPU6050 detects hand tilt and movement.
2. ATmega16 reads sensor values using I2C communication.
3. The microcontroller processes X, Y, and Z axis data.
4. Directional commands are generated:
   - Forward
   - Backward
   - Left
   - Right
   - Stop
5. Commands are transmitted wirelessly using HC-05 via UART.

### Receiver Side

1. HC-05 receives Bluetooth commands.
2. ATmega16 processes the received data.
3. L293D motor driver controls the DC motors.
4. The robotic car moves according to hand gestures.

---

## Communication Protocols Used

### I2C Communication
Used for:
- MPU6050 sensor interfacing

### UART Communication
Used for:
- HC-05 Bluetooth communication

---

## Pin Connections

### MPU6050 to ATmega16

| MPU6050 | ATmega16 |
|---|---|
| VCC | 5V |
| GND | GND |
| SDA | SDA |
| SCL | SCL |

### HC-05 to ATmega16

| HC-05 | ATmega16 |
|---|---|
| TX | RX |
| RX | TX |
| VCC | 5V |
| GND | GND |

### L293D to ATmega16

| L293D | ATmega16 |
|---|---|
| IN1 | PD0 |
| IN2 | PD1 |
| IN3 | PD2 |
| IN4 | PD3 |

---

## Software Used

- AVR GCC
- Atmel Studio / Microchip Studio
- Proteus (for simulation)
- Embedded C

---

## Project Applications

- Gesture-controlled robotics
- Industrial automation
- Wireless robotic vehicles
- Military surveillance robots
- Smart wheelchair control
- Assistive robotic systems

---

## Resume Description

Designed and developed a gesture-controlled 4WD remote car using ATmega16, processing MPU6050 IMU data to enable real-time motion-based vehicle navigation. Implemented bare-metal Embedded C firmware with low-level I2C (MPU6050) and UART (HC-05 Bluetooth) drivers, achieving wireless gesture transmission and low-latency motor control using L293D motor drivers.

---

## Future Improvements

- Obstacle avoidance using ultrasonic sensors
- Mobile app-based control support
- GPS tracking integration
- Camera-based live monitoring
- Wi-Fi control using ESP32
- OTA firmware update support

---

## Author

Kishan Shivhare

Embedded Systems | Firmware Development | STM32 | ATmega | CAN | UART | Bluetooth | IoT
