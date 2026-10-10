[Motion Detection Alarm Code.docx](https://github.com/user-attachments/files/33292040/Motion.Detection.Alarm.Code.docx)
<img width="1845" height="1163" alt="Motion Detection Alarm Daigram" src="https://github.com/user-attachments/assets/d4e602f9-95f5-432a-973c-7dc5d9684927" />
# arduino-ultrasonic-motion-detection-alarm
arduino-ultrasonic-motion-detection-alarm
2. Components identified from your code

Arduino board — exact model to confirm

Ultrasonic distance sensor — trigger pin 9, echo pin 10

Servo motor — pin 6

Green LED — pin 2

Red LED — pin 3

Buzzer — pin 4

16×2 I2C LCD — address 0x27

Breadboard and jumper wires, if used in your build
# Ultrasonic Motion Detection Alarm

An Arduino-based detection and alert system that uses ultrasonic distance measurement, servo scanning, an I2C LCD, LEDs, and a buzzer.

## Project Overview

This project continuously measures the distance to nearby objects. When an object is detected within the configured 20 cm threshold, the system activates a warning display, red LED, and buzzer. When no object is detected within that threshold, the green LED turns on and the servo continues moving between its scanning positions.

## Components Used

* Arduino-compatible microcontroller board
* Ultrasonic distance sensor
* Servo motor
* 16×2 LCD with I2C interface
* Green LED
* Red LED
* Buzzer
* Breadboard and jumper wires, if used

## Features

* Ultrasonic distance measurement
* Configurable 20 cm detection threshold
* Servo-based scanning movement
* LCD status messages
* LED status indication
* Audible warning through a buzzer

## Pin Connections

| Component       | Arduino pin |
| --------------- | ----------- |
| Ultrasonic TRIG | D9          |
| Ultrasonic ECHO | D10         |
| Green LED       | D2          |
| Red LED         | D3          |
| Buzzer          | D4          |
| Servo signal    | D6          |
| LCD I2C address | 0x27        |

The LCD uses I2C communication. Confirm the board's SDA and SCL pins and the actual wiring before assembly.

## Software Requirements

* Arduino IDE
* `Wire` library
* `LiquidCrystal_I2C` library compatible with the code
* `Servo` library

## How It Works

1. The ultrasonic sensor measures the distance to an object.
2. If the measured distance is greater than 20 cm, or the reading is zero, the system displays an empty-area message and activates the green LED.
3. The servo moves between positions to provide a scanning effect.
4. If an object is detected at a distance of 20 cm or less, the red LED and buzzer activate.
5. The LCD displays a warning message while the servo holds its current position.

## Installation

1. Install the Arduino IDE.
2. Install the required LCD library.
3. Connect the components according to the verified circuit diagram.
4. Open the `.ino` source file.
5. Select the correct board and port.
6. Upload the sketch.
7. Test distance readings, LCD messages, LEDs, buzzer, and servo operation.

## Project Status

* Source code: Available
* Circuit diagram: Add the actual diagram to this repository
* Compilation and hardware testing: Record results after testing

## Safety and Limitations

This is an educational prototype, not a certified security alarm. Detection performance depends on sensor placement, object characteristics, wiring, and environmental conditions.

## Author

**Imran Khan**

* GitHub: https://github.com/Imran-khan009
* Portfolio: https://sengrimrankhan.netlify.app
![Uploading Motion Detection Alarm Daigram.png…]()
