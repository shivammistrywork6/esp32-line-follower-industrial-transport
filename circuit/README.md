# Circuit Architecture and System Connections

## 1. System Overview

The line-following robot uses an ESP32 microcontroller to process signals from an infrared (IR) sensor array and control two DC motors through an L293D motor driver.

The robot follows a predefined path using the contrast between a dark line and a lighter floor.

## 2. Main Electrical Components

| Component | Function |
|---|---|
| ESP32 | Main microcontroller and decision-making unit |
| IR sensor array | Detects the line position |
| L293D motor driver | Controls the DC motors |
| Two DC motors | Provide locomotion |
| Rechargeable LiPo battery cells | Supply electrical power |
| Switch | Controls power to the system |
| Jumper wires and connectors | Provide electrical connections |

## 3. Functional Signal Flow

1. The IR sensors detect the surface beneath the robot.
2. Sensor outputs are received by the ESP32.
3. The ESP32 processes the sensor information.
4. Control signals are sent to the L293D motor driver.
5. The motor driver controls the two DC motors.
6. The robot adjusts its movement to follow the line.

## 4. Movement Logic

| Detected condition | Intended robot response |
|---|---|
| Centre sensor detects the line | Move straight |
| Left side detects the line | Adjust towards the left |
| Right side detects the line | Adjust towards the right |
| Line is lost | Stop |
| Junction or all sensors detect the line | Stop |

*Note: This table describes the intended operating logic documented for the project. Exact pin assignments and motor-control implementation should be added after verification.*

## 5. Future Improvements

- Implement PID-based line-following control.
- Add obstacle-detection sensors.
- Improve wiring reliability and connection security.
- Explore higher-torque geared motors.
- Develop a detailed circuit schematic with verified pin assignments.
