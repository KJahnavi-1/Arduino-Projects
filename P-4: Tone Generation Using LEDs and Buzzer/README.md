# 🔔 Tone Generation Using LEDs and Buzzer

This Arduino project demonstrates how to combine **LEDs** and a **buzzer** to produce different tones based on which LED is active. Each LED (Red, Yellow, Green) corresponds to a specific tone, creating a synchronized light-and-sound effect.

---

## 🔧 Components Required

- 1 x Arduino Uno (or compatible board)  
- 3 x LEDs (Red, Yellow, Green)  
- 3 x 220Ω resistors  
- 1 x Piezo Buzzer  
- Breadboard and jumper wires  

---

## 🔌 Circuit Diagram

| Component     | Arduino Pin |
|---------------|-------------|
| Red LED       | 13          |
| Yellow LED    | 12          |
| Green LED     | 11          |
| Buzzer (+ve)  | 7           |
| Buzzer (-ve)  | GND         |

> Connect a 220Ω resistor in series with each LED to limit current.

---

## 🧠 How It Works

- The buzzer is used in combination with `tone()` to generate sound.
- Each LED corresponds to a different tone:
  - 🔴 Red LED → 500 Hz
  - 🟡 Yellow LED → 1000 Hz
  - 🟢 Green LED → 1500 Hz
- When an LED is ON, the buzzer plays the associated tone.
- Each combination remains active for 2 seconds.

---
