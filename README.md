# Robotics — Fall 2026

## Week 4: Line Following with PD Control

This TRIK Studio project uses two light sensors to follow a black line. The robot continuously compares the sensor readings and adjusts the two motor powers to steer along the path.

### How it works

- **Sensor calibration:** Each sensor's white and black readings are converted to a common scale, allowing sensors with different sensitivities to be compared fairly.
- **Proportional control (P):** Corrects the current sensor imbalance. A larger error requests stronger steering.
- **Derivative control (D):** Responds to changes in error to help reduce overshoot.
- **Motor control:** Both motors run at the same base power when the error is zero. Different powers produce a turn, with the steering correction limited to avoid excessive commands.

### Running the project

Open the `.qrs` file in TRIK Studio. Check the sensor ports and wheel assignments, position the robot on the line, and start the program. For physical testing, calibrate the sensors using the actual track and lighting conditions.
