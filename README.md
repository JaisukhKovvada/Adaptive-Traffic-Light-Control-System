# Adaptive Traffic Light Control System

## Overview

This project implements an adaptive traffic light control system using Arduino and IR sensors. Instead of using fixed traffic signal timings, the controller continuously monitors vehicle density on two roads and dynamically assigns the green signal to the road with higher traffic.

The system demonstrates how embedded systems and real-time decision-making algorithms can improve traffic flow efficiency.

---

## Features

- Real-time vehicle counting using IR sensors
- Dynamic traffic density comparison
- Adaptive green signal allocation
- Rule-based embedded control logic
- Simple and scalable design
- Arduino implementation

---

## Components Used

- Arduino Uno
- 4 IR Sensors
- LEDs
- Jumper Wires
- Breadboard
- USB Cable

---

## Working Principle

1. Vehicles entering Road A and Road B are detected by entry IR sensors.
2. Exit sensors decrement the vehicle count after vehicles leave.
3. The controller continuously compares traffic density.
4. The road with higher traffic receives the green signal.
5. If both roads have equal traffic, both signals remain off.

---

## Pin Configuration

| Component | Arduino Pin |
|-----------|-------------|
| IR A Entry | D2 |
| IR A Exit | D3 |
| IR B Entry | D4 |
| IR B Exit | D5 |
| Green LED A | D8 |
| Green LED B | D11 |

---

## Algorithm

1. Initialize sensors and LEDs.
2. Detect vehicle entry.
3. Increment corresponding road counter.
4. Detect vehicle exit.
5. Decrement vehicle counter.
6. Compare traffic counts.
7. Assign green signal to the road with higher traffic.
8. Repeat continuously.

---

## Project Structure

```
Adaptive-Traffic-Light-Control-System

│
├── Arduino_Code
│     adaptive_traffic.ino
│
├── Circuit_Diagram
│
├── Images
│
└── README.md
```

---

## Future Improvements

- Four-road intersection support
- Emergency vehicle detection
- IoT monitoring dashboard
- Machine Learning based traffic prediction
- GSM notification system

---

## Author

Jaisukh Kovvada
Electronics and Communication Engineering
