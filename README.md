# Arduino Radar Detector

## Project Overview
This project demonstrates how to build a simple radar detection system using Arduino components. The system scans its environment by rotating the ultrasonic sensor and measuring distances to objects, providing real-time data that can be visualized using external software.

## Components Used
- **Arduino Board (e.g., Arduino Uno):** The microcontroller that controls the radar system.  
- **HC-SR04 Ultrasonic Sensor:** Measures distances by emitting ultrasonic waves and calculating the time taken for the echo to return.  
- **SG90 Servo Motor:** Rotates the ultrasonic sensor across a specified angle range to scan the environment.  
- **External Software (e.g., Processing):** Visualizes the radar data in real-time, displaying a radar-like interface.  

## How It Works
1. **Initialization:** The servo motor is set to an initial position, and the ultrasonic sensor is prepared for measurements.  
2. **Scanning:** The servo motor rotates the sensor across a specified angle range (e.g., 0° to 180°).  
3. **Distance Measurement:** At each position, the ultrasonic sensor measures the distance to the nearest object.  
4. **Data Output:** The angle and corresponding distance are sent to the serial monitor in a comma-separated format (e.g., `angle,distance`).  
5. **Visualization:** External software reads the serial data and visualizes it as a radar display, updating in real-time.
