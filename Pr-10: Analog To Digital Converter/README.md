# Analog Sensor Input to Sound Frequency (Buzzer)

This project demonstrates how to use an **analog sensor** (like a potentiometer, LDR, or any analog sensor) with Arduino and generate different **sound frequencies** using a buzzer.  
The sensor values are mapped to a frequency range, and the buzzer outputs tones accordingly.

---

## 📖 Overview
- The analog sensor connected to **A0** provides values from **0 to 1023**.  
- These values are mapped to a **frequency range (100 Hz to 2000 Hz)**.  
- If the sensor is active, a tone is played on pin **13**; otherwise, the buzzer remains silent.  
- The sensor readings are also displayed in the **Serial Monitor** at `115200 baud`.  

---

## 🛠 Components Required
- Arduino Uno  
- Buzzer (active/passive)  
- Analog Sensor (e.g., potentiometer, LDR, microphone module, etc.)  
- Resistors (if required for sensor)  
- Breadboard & Jumper Wires  

---

## ⚡ Circuit Diagram
- Sensor output → A0  
- Buzzer → Pin 13  
- Sensor VCC → 5V  
- Sensor GND → GND  

*(Insert your TinkerCad/real circuit diagram here)*

---

## 🔑 Working Principle
1. The sensor provides an analog input ranging from **0 to 1023**.  
2. Arduino reads this input and maps it into a frequency range **100 Hz – 2000 Hz**.  
3. The buzzer connected to **Pin 13** plays the corresponding tone.  
4. If the sensor gives no input (`0`), the buzzer turns OFF.  
5. Sensor readings are printed on the **Serial Monitor** for observation.  

---

## 🚀 Applications
- Sound-based sensor feedback systems  
- Musical experiments using sensors  
- Interactive learning projects  
- Real-time analog signal monitoring  
