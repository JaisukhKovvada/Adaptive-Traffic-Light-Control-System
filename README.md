Adaptive Traffic Light Control System
Overview 

This project implements an intelligent traffic light control system using Arduino and IR sensors. Instead of assigning fixed signal timings, the system continuously monitors vehicle density on two roads and dynamically grants the green signal to the road with higher traffic.

The objective is to reduce unnecessary waiting time, improve traffic flow, and demonstrate a simple adaptive traffic management approach using embedded systems.

Features
Real-time vehicle counting using IR sensors
Adaptive signal control based on traffic density
Rule-based decision-making algorithm
Edge detection to avoid multiple counts
Low-cost embedded implementation
Easily expandable for multiple intersections
Components Used
Arduino UNO
IR Sensors (4)
LEDs
Breadboard
Jumper Wires
USB Cable
Working Principle
IR sensors detect vehicles entering and leaving each road.
Vehicle counts are updated in real time.
The controller compares traffic density on both roads.
The road with higher traffic receives the green signal.
Signal status continuously updates as traffic changes.
Algorithm
Initialize sensors and LEDs

Loop forever

Read all IR sensors

If vehicle enters Road A
    Increment Count A

If vehicle exits Road A
    Decrement Count A

If vehicle enters Road B
    Increment Count B

If vehicle exits Road B
    Decrement Count B

Compare Count A and Count B

If Count A > Count B
    Give Green to Road A

Else If Count B > Count A
    Give Green to Road B

Else
    Keep both signals OFF

Repeat
Technologies Used
Arduino IDE
Embedded C
Arduino UNO
IR Sensors
Rule-Based Control Logic
Future Improvements
Emergency vehicle priority
GSM notification
IoT monitoring
Machine Learning based prediction
Multiple junction support
Author

Jaisukh Kovvada
