Line Following Waiter Robot

The Line Following Waiter Robot is an autonomous embedded robotics system designed to operate in structured environments such as restaurants or service areas. It is capable of navigating predefined paths, identifying customer tables, delivering items, and returning to its docking station without human intervention.

The system integrates motion control, computer vision, sensor fusion, and wireless communication using a distributed multi-microcontroller architecture.

🚀 Key Features
Autonomous line-following using 5-channel IR sensor array
PID control algorithm for stable and accurate path tracking
Autonomous mapping using Left-Hand Rule navigation
Path recording and retrieval using encoder-based memory system
AI-based table detection using ESP32-CAM + Edge Impulse model
Real-time obstacle avoidance using ultrasonic sensing (HC-SR04)
Battery monitoring using INA219 power sensor
Wireless control via Bluetooth + Wi-Fi WebSocket dashboard
Fully autonomous delivery and return-to-dock system
🧠 System Architecture

The robot is built using a three-board distributed architecture:

Arduino Uno (ATmega328P): Motion control, motor driving, PID line following
ESP32 DevKit: Sensor fusion, communication, telemetry, system coordination
ESP32-CAM: Machine learning-based vision for table identification
⚙️ Working Principle

The robot operates in two main phases:

1. Mapping Phase
Explores the environment using Left-Hand Rule algorithm
Detects junctions and records movement path
Identifies table markers using grayscale classification
Stores navigation data on SD card
2. Delivery Phase
Navigates to selected destination table
Confirms arrival using AI vision model
Executes delivery and dwell time
Retraces stored path back to docking station
🔋 Hardware Overview
Arduino Uno (ATmega328P)
ESP32 DevKit V1
ESP32-CAM module
TCRT5000 IR Sensor Array (5-channel)
HC-SR04 Ultrasonic Sensor
INA219 Voltage/Current Sensor
LM2596 Buck Converter
3×18650 Li-ion Battery Pack (11.1V)
16×2 LCD Display
📡 Communication Systems
Bluetooth Classic (mobile control & commands)
Wi-Fi WebSocket (real-time monitoring dashboard)
🎥 Project Demo

Add your YouTube video here:

https://www.youtube.com/watch?v=YOUR_VIDEO_ID
📄 Documentation

Full project report is available in the /report folder.

💡 Applications
Smart restaurants and automated food delivery systems
Industrial internal logistics systems
Autonomous service robotics research
Embedded AI + IoT integration projects
🔧 Future Improvements
SLAM-based mapping instead of rule-based navigation
Improved object recognition with deep learning models
Cloud-based telemetry dashboard
Voice interaction system for orders
