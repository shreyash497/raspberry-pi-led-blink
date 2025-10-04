# raspberry-pi-led-blink
Simple Raspberry Pi LED blink experiment using Python to control GPIO pins. Demonstrates basic hardware interfacing and hands-on lab skills.
# 💡 Raspberry Pi LED Blink Experiment

This repository documents a simple **LED Blink experiment** performed using a **Raspberry Pi**.  
The goal was to control an LED through the Raspberry Pi’s GPIO pins using Python.

---

## 🧰 Hardware Used
- Raspberry Pi (Model used: Raspberry Pi 3B / 4B)
- 1 × LED
- Jumper wires
  

---

## ⚙️ Circuit Connection
| Component | Raspberry Pi Pin | Description |
|------------|------------------|--------------|
| LED (Anode +) | GPIO17 (Pin 11) | Output pin controlling LED |
| LED (Cathode -) | GND | Direct connection |

---

# 💻 Software & Programming
- Operating System:** Raspberry Pi OS  
- Language:** Python  
- Library:** `RPi.GPIO` or `gpiozero`

> 🕒 *Code will be added later once retrieved from the lab system.*
> from gpiozero import LED
from time import sleep

# Use GPIO17 (Pin 11 on Raspberry Pi)
led = LED(17)

print("LED Blink Program Started... Press Ctrl+C to stop.")

try:
    while True:
        led.on()          # Turn LED ON
        print("LED ON")
        sleep(1)          # Wait 1 second
        led.off()         # Turn LED OFF
        print("LED OFF")
        sleep(1)          # Wait 1 second
except KeyboardInterrupt:
    print("\nProgram stopped by user.")


---

## 📸 Experiment Photos

| LED Blink | Breadboard Setup |
|------------|------------------|
| ![LED Blink](images/led_blink_1.jpg) | ![Setup](images/led_blink_2.jpg) |

---

## 🧠 What I Learned
- How to control GPIO pins in Raspberry Pi using Python  
- Basics of interfacing LEDs and simple circuits  
- Understanding the importance of current-limiting resistors in future setups  



