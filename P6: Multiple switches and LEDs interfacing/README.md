# 🔘 Multiple Switches and LEDs Interfacing

This Arduino project demonstrates how to **control multiple LEDs using multiple push buttons**. Each button is mapped to one LED, allowing independent control:
- Pressing **Switch 1** → Turns ON **LED 1**  
- Pressing **Switch 2** → Turns ON **LED 2**  
- Releasing a switch → Turns OFF the corresponding LED  

This project expands on the basics of digital input/output by handling more than one input simultaneously.

---

## 🔧 Components Required

- 1 x Arduino Uno (or compatible board)  
- 2 x LEDs (any color)  
- 2 x 220Ω resistors (for LEDs)  
- 2 x Push buttons  
- 2 x 10kΩ resistors (for button pull-downs)  
- Breadboard and jumper wires  

---

## 🔌 Circuit Diagram

**Connections:**
- **LEDs**  
  - LED1 (with 220Ω resistor) → Pin 12  
  - LED2 (with 220Ω resistor) → Pin 11  

- **Switches**  
  - Switch1 → Pin 6 (with 10kΩ resistor to GND)  
  - Switch2 → Pin 5 (with 10kΩ resistor to GND)  

---

## 🧠 How It Works

- Each switch is connected to an **Arduino input pin**.  
- The state of the switches is read using `digitalRead()`.  
- If a switch is pressed (`HIGH`), the corresponding LED turns **ON**.  
- If released (`LOW`), the LED turns **OFF**.  
- A short delay (`50 ms`) is included to minimize the effect of **switch bouncing**.  

---
