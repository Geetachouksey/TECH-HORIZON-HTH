# Mood Align  
*A Smart Stress Detection & Health Monitoring Device*

Mood Align is a health monitoring device designed for patients to help detect **stress levels**, **heart rate**, and provide **real-time visualization** on an OLED display. The system uses biomedical sensors such as **SPO2**, **ECG**, and **IR sensors**. It also supports **wireless relay triggering** for automation and alert purposes. The main controller used is the **Raspberry Pi Pico W**.

---

## Features
- 🫀 Real-time **heart rate monitoring** using ECG sensor  
- 🌬 **SpO2 & stress level detection** with OLED display indication  
- 📊 **Graphical plotting** of heart rate and stress levels on OLED  
- 📡 **Wireless relay triggering** based on sensor inputs  
- 🔌 Powered by **Raspberry Pi Pico W** (low power + Wi-Fi support)  

---

## Components Used
- Raspberry Pi Pico W (Main Controller)  
- MAX30100 / MAX30102 SpO2 & Heart Rate Sensor  
- ECG Sensor Module (AD8232 or similar)  
- IR Sensor  
- OLED Display (SH1106 / SSD1306, I2C)  
- Wireless Relay Module  
- Jumper wires and power supply  

---

## Block Diagram
[ECG Sensor] →
[SpO2 Sensor] → [Raspberry Pi Pico W] → [OLED Display]
[IR Sensor] → ↓
[Relay Trigger] ←────────────────────
---

## Installation & Setup
Clone the repository and upload the code to Raspberry Pi Pico W using **Thonny IDE** with **MicroPython firmware**. Ensure required libraries are included on the Pico W filesystem (`ssd1306.py` or `sh1106.py` for OLED, additional drivers for sensors). Run the `main.py` script to start monitoring.

---

## Future Enhancements
- Cloud connectivity for remote health monitoring  
- Mobile application for real-time stress and heart data visualization  
- AI-based stress prediction with recommendations  

---

## Contributing
Contributions, issues, and feature requests are welcome. Feel free to fork this repository and submit pull requests.  

---

## License
This project is licensed under the MIT License – see the LICENSE file for details.  
