# Testing and Performance Evaluation

## 1. Testing Objective

The objective of testing is to evaluate the line-following robot's ability to detect a predefined path and adjust its movement using its IR sensor array and ESP32-based control system.

## 2. Functional Testing

The following functional behaviours are considered during evaluation:

| Test | Expected behaviour |
|---|---|
| Straight-line tracking | Robot maintains forward movement along the line |
| Left deviation | Robot adjusts its direction towards the left |
| Right deviation | Robot adjusts its direction towards the right |
| Line loss | Robot stops when the line is no longer detected |
| Junction detection | Robot stops when the documented junction condition is detected |

## 3. Observed Project Limitations

The following limitations were identified during project development:

- Performance depends on sufficient contrast between the line and the floor.
- Loose jumper-wire connections can affect reliability.
- The prototype does not include obstacle-detection capability.
- Payload capacity is limited.

## 4. Future Performance Improvements

- Implement PID-based control for smoother tracking.
- Add obstacle-detection sensors.
- Improve electrical connections and wiring management.
- Evaluate stronger geared motors for improved torque.
- Conduct systematic testing across different track geometries.

## 5. Experimental Results

Detailed quantitative results, such as tracking accuracy, speed, response time and successful run percentage, can be added after controlled testing.

No quantitative performance figures are claimed in this document.
