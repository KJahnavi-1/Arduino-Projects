# Arduino Programming with LCD

## 📌 Overview
This project demonstrates how to interface a **16x2 LCD display** with an **Arduino Uno** using the `LiquidCrystal` library.  
The LCD displays a custom welcome message, scrolls it across the screen, and then shows a real-time counter (seconds since the Arduino was reset).

---

## 🛠️ Components Required
- Arduino Uno  
- 16x2 LCD Display (HD44780 or compatible)  
- 10kΩ Potentiometer (for contrast adjustment) *(optional but recommended)*  
- 220Ω Resistor (for LCD backlight LED)  
- Breadboard  
- Jumper wires  

---


### Wiring Table

| LCD Pin | Arduino Pin | Description |
|---------|-------------|-------------|
| VSS     | GND         | Ground |
| VDD     | 5V          | Power supply |
| V0      | Potentiometer | Contrast control |
| RS      | 13          | Register Select |
| E       | 12          | Enable |
| D4      | 5           | Data pin |
| D5      | 4           | Data pin |
| D6      | 3           | Data pin |
| D7      | 2           | Data pin |
| A (LED+) | 5V (via 220Ω) | Backlight anode |
| K (LED–) | GND         | Backlight cathode |

---

## 📖 Explanation

This project demonstrates the working of a **16x2 LCD** with Arduino using the `LiquidCrystal` library. Below is the step-by-step explanation:

1. **Initialization**  
   - The LCD is initialized with pins RS=13, EN=12, D4=5, D5=4, D6=3, D7=2.  
   - The `lcd.begin(16, 2);` command sets the LCD to 16 columns and 2 rows.

2. **Displaying a Welcome Message**  
   - The message `"Hello, I'm Jahnavi Korivi!"` is printed on the first row of the LCD.  
   - A short delay is added to let the text appear clearly.

3. **Scrolling Effect**  
   - The text scrolls **to the left** across the display.  
   - This is done using `lcd.scrollDisplayLeft();` inside a loop with a 200ms delay.  
   - It creates a moving text effect.

4. **Clearing the Display**  
   - After scrolling, the screen is cleared using `lcd.clear();`.  
   - A new message `"Count:"` is displayed at the beginning of the first row.

5. **Real-Time Counter**  
   - In the `loop()` function, the LCD cursor is placed after `"Count:"`.  
   - The counter uses `millis() / 1000` to show elapsed time in seconds since the Arduino was powered on.  
   - The display updates automatically to show the running count.

---

✅ In short:  
- First, the LCD shows a welcome message.  
- Then, the text scrolls across the screen.  
- Finally, the display shows a live counter of seconds.  

