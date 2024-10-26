<h2>Motion Sensor & Servomotor</h2>
This project demonstrates how to control a servo motor with an ESP32 based on input from a motion sensor. <br>
The servo will rotate to 90 degrees when motion is detected, and return to 0 degrees when no motion is detected.<br>
The motion sensor is connected to pin 25, and the servo is controlled via pin 26.<br>

![circuit diagram](https://github.com/user-attachments/assets/ab364f47-579e-4c83-b05b-d14648b932cf)


<h3>Components Used</h3>
ESP32 microcontroller<br>
Servo motor<br>
PIR motion sensor<br>
Jumper wires<br>
Breadboard<br>

<h3>Libraries Required</h3>
ESP32Servo Library - This library allows for controlling servos using the ESP32.

<h3>Pin Configuration</h3>
Servo Motor Pin: Pin 26
Motion Sensor Pin: Pin 25

<h3>Code Explanation</h3>
Setup:<br>
The serial communication is initialized at 115200 baud rate for debugging purposes.<br>
The servo motor is attached to pin 26, and its initial position is set to 0 degrees.<br>
Pin 25 is configured as an input to read the signal from the motion sensor.<br>

Loop:<br>
The code continuously checks the motion sensor value.<br>
If motion is detected (logic HIGH), the servo rotates to 90 degrees.<br>
If no motion is detected (logic LOW), the servo returns to 0 degrees.<br>
A small delay of 100ms is added to avoid excessive polling.<br>

<h3>How to Use</h3>
Install the ESP32Servo library in your Arduino IDE.<br>
Upload the provided code to your ESP32.<br>
Connect the motion sensor and servo motor as per the pin configuration.<br>
Open the Serial Monitor at 115200 baud rate to see the real-time status.<br>
