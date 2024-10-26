<h2>LED Control</h2>
This Arduino project reads an analog signal from potentiometer and controls four LEDs based on the value of the input. 
The LEDs are connected to pins 12, 14, 27, and 26.<br>

![output](https://github.com/user-attachments/assets/b7a14cf2-a2cf-43d0-a6f8-eb94ef30c42c)


<h3>Hardware Requirements</h3>
Arduino board (ESP32 or similar)<br>
4 LEDs<br>
Potentiometer<br>
Resistors for each LED<br>
Jumper wires<br>
Breadboard<br>

<h3>Pin Configuration</h3>

| Pin | Function |
| ------------- | ------------- |
| 33 | Analog Input (potentiometer) |
| 12 | LED 1 (output) |
| 14  | LED 2 (output)  |
| 27  | LED 3 (output)  |
| 26  | LED 4 (output)  |


<h3>How it Works</h3>
The analog input is read from pin 33 using analogRead().<br>
The value of the input is printed to the serial monitor.<br>
<h5>Depending on the range of the input value, one of the LEDs is turned off while the others remain on:</h5>
500 ≤ pin value ≤ 1000: LED 1 is turned off.<br>
1000 < pin value ≤ 2000: LED 2 is turned off.<br>
2000 < pin value ≤ 3000: LED 3 is turned off.<br>
Otherwise: LED 4 is turned off.<br>
