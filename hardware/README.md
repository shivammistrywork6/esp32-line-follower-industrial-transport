# Hardware Architecture

## 1. Overview

The robot is a compact, differential-drive line-following system developed as part of a Mechatronics Case Study Project at SVNIT Surat.

Its hardware combines sensing, embedded control, motor driving and a mobile chassis to demonstrate automated path following.

## 2. Hardware Components

| Component | Purpose |
|---|---|
| ESP32 development board | Processes sensor inputs and generates motor-control signals |
| IR sensor array | Detects the line using surface contrast |
| L293D motor driver | Interfaces the microcontroller with the DC motors |
| Two DC motors | Drive the left and right wheels |
| Robot chassis | Supports the mechanical and electrical components |
| Rechargeable LiPo battery cells (3) | Provide portable power |
| Power switch | Enables or disables the system |
| General-purpose circuit board (GCB) | Supports electronic connections |
| Jumper wires and connectors | Connect the electronic components |

## 3. System Architecture

The hardware can be divided into four functional subsystems:

1. **Sensing subsystem:** IR sensors detect the line position.
2. **Control subsystem:** The ESP32 processes sensor signals.
3. **Motor-driving subsystem:** The L293D controls the two DC motors.
4. **Mechanical subsystem:** The chassis, wheels and motors provide movement.

## 4. Drive Configuration

The robot uses two independently driven DC motors.

By varying the movement of the left and right motors, the robot can move forward and adjust its direction while following a line.

## 5. Development Considerations

The project demonstrates the integration of mechanical, electrical and embedded systems in a compact mobile robot.

Potential improvements include better wiring management, obstacle detection, PID-based control and higher-torque motors.
