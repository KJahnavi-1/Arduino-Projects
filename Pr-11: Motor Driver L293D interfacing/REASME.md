# Motor Driver L293D Interfacing with Arduino

## Project Overview
This project demonstrates how to interface a DC motor with an Arduino using the L293D motor driver IC. The motor is controlled through a slider switch.  
- When the switch is **ON (HIGH)** → The motor rotates in one direction.  
- When the switch is **OFF (LOW)** → The motor rotates in the opposite direction.  

This setup helps in learning the basics of controlling DC motors in embedded systems and robotics applications.

---

## Components Required
- Arduino Uno  
- L293D Motor Driver IC  
- DC Motor  
- Slider Switch / Push Button  
- Breadboard  
- Jumper Wires  
- Power Supply  

---

## Circuit Connections
1. **Motor Driver (L293D):**
   - Motor is connected to the output pins of the L293D.  
   - Input pins of the L293D are connected to Arduino pins **12** and **13**.  
   - Enable pin is powered via Vcc and GND.  

2. **Slider Switch:**
   - Connected to Arduino pin **6** as input.  

3. **Arduino to L293D:**
   - `motorPin1` → Pin 13  
   - `motorPin2` → Pin 12  

4. **Power Supply:**
   - Arduino powered via USB.  
   - Motor powered through external supply via the L293D.  

---

## Working Principle
- The slider switch acts as the control input.  
- If the slider switch is pressed (**HIGH**):  
  - Motor rotates in one direction (`motorPin1 = HIGH, motorPin2 = LOW`).  
- If the slider switch is released (**LOW**):  
  - Motor rotates in the opposite direction (`motorPin1 = LOW, motorPin2 = HIGH`).  

---

## Circuit Diagram
Circuit representation created in TinkerCAD:  

![Circuit Diagram](Screenshot%202025-09-05%20204225.png)

---

## Applications
- Basic robotics (motor direction control).  
- Conveyor belts and small automation systems.  
- Learning motor driver ICs in embedded systems.  
