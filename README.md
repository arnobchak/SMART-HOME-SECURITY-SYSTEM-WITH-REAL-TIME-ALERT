# SMART HOME SECURITY SYSTEM WITH REAL-TIME ALERT

## Project Overview
This project demonstrates the development of a smart home security system that provides real-time alerts. By leveraging an ESP32-CAM module, PIR motion sensor, LED indicators, and other components, this system can detect motion and capture images, sending alerts in real-time to enhance home security.

## Features
- Motion detection using a PIR sensor.
- Real-time image capture with the ESP32-CAM module.
- LED indicators for system status.
- Alert notifications sent via email or other communication channels.
- Low-cost and scalable design for smart home integration.

---

## Components Used
1. **ESP32-CAM Module** - For image capturing and processing.
2. **PIR Sensor** - To detect motion in the monitored area.
3. **BC547 NPN Transistor** - Used for switching purposes.
4. **Resistors**:
   - 220 Ohm
   - 1k Ohm
   - 10k Ohm
5. **LED Indicator** - To display system status (e.g., motion detected, capturing image).
6. **FTDI 232 USB to Serial Interface Board** - For programming the ESP32-CAM module.
7. **5V DC Power Supply** - To power the system components.

---

## Circuit Diagram
To visualize the connections, refer to the circuit diagram below:
1. Connect the PIR sensor to the ESP32-CAM for motion detection.
2. Use the BC547 transistor and resistors to control the LED indicator.
3. Power the entire system using a 5V DC power supply.

> **Note**: A detailed circuit diagram will be provided in the `Diagrams` folder of this repository.

---

## Installation and Setup
1. **Hardware Setup**:
   - Connect the components as per the circuit diagram.
   - Ensure proper connections and power supply to the ESP32-CAM and peripherals.

2. **Software Requirements**:
   - Arduino IDE or PlatformIO.
   - ESP32 board support package installed in the IDE.
   - Necessary libraries (e.g., `ESP32-CAM`, `WiFi`, `SMTP`).

3. **Programming the ESP32-CAM**:
   - Connect the FTDI 232 USB to Serial Interface Board to the ESP32-CAM.
   - Load the provided code from the `Code` folder into the Arduino IDE.
   - Configure your Wi-Fi credentials and email/alert settings in the code.
   - Upload the code to the ESP32-CAM module.

---

## Usage
1. Power on the system using a 5V DC power supply.
2. When motion is detected by the PIR sensor, the ESP32-CAM captures an image.
3. The LED indicator lights up, signaling that motion has been detected.
4. The captured image is sent as an email or alert notification in real-time.

---

## Repository Structure
```
SMART-HOME-SECURITY-SYSTEM-WITH-REAL-TIME-ALERT/
|
├── Code/
|   └── smart_home_security.ino   # Arduino code for the ESP32-CAM
|
├── Diagrams/
|   └── circuit_diagram.png       # Circuit connection diagram
|
├── Images/
|   └── demo_screenshot.jpg       # Example of captured images
|
├── README.md                     # Project documentation
|
└── LICENSE                       # Project license
```

---

## Future Enhancements
- Integration with IoT platforms like MQTT or Firebase for cloud-based monitoring.
- Adding a buzzer alarm for audible alerts.
- Enhancing the system with night vision capabilities using IR LEDs.
- Implementing a mobile application for remote control and monitoring.

---

## Contribution
Contributions to this project are welcome! Feel free to open issues or submit pull requests to improve the design, functionality, or documentation.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

## Acknowledgments
- Thanks to the open-source community for providing libraries and tools.
- Special thanks to those who contributed to the development of the ESP32-CAM ecosystem.

