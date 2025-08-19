# 🔢 Interfacing 7-Segment LED Display

This Arduino project demonstrates how to **interface and control a 7-Segment LED display**.  
It sequentially displays numbers **0 to 9**, with each digit staying visible for 1 second before switching to the next.

---

## 🔧 Components Required

- 1 x Arduino Uno (or compatible board)  
- 1 x Common Cathode 7-Segment Display  
- 2 x 220Ω resistors   
- Breadboard and jumper wires  

---

## 🔌 Circuit Connections

**Arduino to 7-Segment Display (Common Cathode):**

| Segment | Arduino Pin |
|---------|-------------|
| A       | 5           |
| B       | 4           |
| C       | 9           |
| D       | 10          |
| E       | 11          |
| F       | 3           |
| G       | 2           |
| COM (Cathode) | GND   |


---

## 🧠 How It Works

- Each segment of the 7-Segment display is controlled by an Arduino pin.  
- A **HIGH signal** turns a segment ON, while **LOW** turns it OFF.  
- Functions (`zero()`, `one()`, … `nine()`) define which segments light up for each digit.  
- The `loop()` function calls these digit functions sequentially with a **1-second delay**.  
- This creates a simple **digital counter (0–9)**.  

---

}

