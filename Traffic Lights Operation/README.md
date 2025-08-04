# 🚦 Traffic Lights Operation

This Arduino project simulates a **traffic signal system** using three LEDs—red, yellow, and green. It models a simple time-based traffic light logic, making it a great beginner project to understand pin control, timing, and sequencing.

---

## 🔧 Components Required

- 1 x Arduino Uno (or compatible board)
- 1 x Red LED  
- 1 x Yellow LED  
- 1 x Green LED  
- 3 x 220Ω resistors  
- Breadboard and jumper wires

---

## 🔌 Circuit Diagram

Connect each LED to its corresponding pin via a resistor:

- Arduino Pin 13 ───► [220Ω Resistor] ───► [Red LED Anode]
- Arduino Pin 11 ───► [220Ω Resistor] ───► [Yellow LED Anode]
- Arduino Pin 9 ───► [220Ω Resistor] ───► [Green LED Anode]
- All LED Cathodes ───► GND

## 🧠 How It Works

The code cycles through three LEDs with equal time delays:
1. **Red LED ON** – Stop
2. **Yellow LED ON** – Get ready
3. **Green LED ON** – Go

Each state lasts for 5 seconds (5000 milliseconds).

---

[Watch the Vedio Explanation of the Project](https://drive.google.com/file/d/1COCRlVW71ievovEIkC4szjivnqxL3zwS/view?usp=drive_link)
