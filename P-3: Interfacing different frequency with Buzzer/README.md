# 🔊 Interfacing Different Frequencies with a Buzzer

This Arduino project demonstrates how to **generate tones of different frequencies using a buzzer**. It uses the `tone()` and `noTone()` functions to produce audible sound patterns that change every second.

---

## 🔧 Components Required

- 1 x Arduino Uno (or compatible board)  
- 1 x Piezo Buzzer  
- 1 x 220Ω resistor (optional, for current limiting)  
- Jumper wires  
- Breadboard  

---

## 🔌 Circuit Connection

- Arduino Pin 13 ───► Buzzer +ve
- Buzzer -ve ───► GND
- Resistor ───► 220Ω 

---

## 🧠 How It Works

- The `tone(pin, frequency)` function is used to generate a square wave of the specified frequency on the given pin.
- `noTone(pin)` stops the sound.
- In this project, the buzzer cycles through tones of **100 Hz**, **500 Hz**, and **900 Hz**, each lasting **1 second**, followed by **2 seconds of silence**.

---

[Watch the Video Explanation of the Project](https://drive.google.com/file/d/1lsQtqTc447JCi7UK8ulAVlAs7znk1ZsO/view?usp=drive_link)
