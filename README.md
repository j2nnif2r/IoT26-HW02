# IoT26-HW01
Gachon Univ. IoT Team F HW01

## Project Overview
This project demonstrates how to read digital inputs using a Raspberry Pi.  
A push button is used as an input device, and an LED is controlled based on the button state using Python.

---

## Objective
- Learn how to read digital input from GPIO pins
- Interface a push button with Raspberry Pi
- Control an LED based on input signal

---

## Hardware Setup
- Raspberry Pi
- Breadboard
- Push button
- LED
- Resistor
- Jumper wires

---

## Circuit
- Push button connected to GPIO input pin
- LED connected to GPIO output pin
- Resistors used for proper current control
- 
<img src="https://github.com/user-attachments/assets/a6c5d33b-f292-4a16-9090-834e2e659b8c" width="400" />

## IDE / Terminal
<img src="https://github.com/user-attachments/assets/aeba832a-8e2e-49f1-b3f0-85cb515cced1" width="400" />


---
## 🎥 Video
[https://youtube.com/shorts/zQwlU01Qszo?feature=share](https://www.youtube.com/shorts/cOuC-Jbngg4?feature=share)

---

## Code
```python
from gpiozero import Button, LED
from signal import pause

button = Button(2)
led = LED(17)

button.when_pressed = led.on
button.when_released = led.off

pause()
```

---
## Team Roles
- **Raspberry Pi Setup**: 김채윤, 김현보  
  (Raspberry Pi connection and development environment setup)

- **Development**: 김건
  (Code execution and refactoring, version synchronization)

- **Documentation**: 김현보
  (Video recording and GitHub repository organization)
