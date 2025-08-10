# 🔘 Interfacing Push Button to LED

This Arduino project demonstrates how to **control an LED using a push button**. When the button is pressed, the LED turns ON; when released, the LED turns OFF. This is one of the most basic and essential beginner projects for learning digital input and output.

---

## 🔧 Components Required

- 1 x Arduino Uno (or compatible board)  
- 1 x Push button  
- 1 x LED  
- 1 x 220Ω resistor (for the LED)  
- 1 x 10kΩ resistor (for the button pull-down)  
- Breadboard and jumper wires  

---

## 🔌 Circuit Diagram

**Connections:**
- Push button → Pin 5 (with 10kΩ resistor to GND as pull-down)  
- LED (Anode) → Pin 13 through 220Ω resistor  
- LED Cathode → GND  

---

## 🧠 How It Works

- The push button is connected to **digital pin 5** as an input.
- The LED is connected to **digital pin 13** as an output.
- `digitalRead(5)` checks the state of the button:
  - If **HIGH** → LED turns ON  
  - If **LOW** → LED turns OFF  

---

[Video Explanation](https://drive.google.com/file/d/1mfc_1L0iGoZe-ito-7WvHrK_TlPZkk9B/view?usp=drive_link)
