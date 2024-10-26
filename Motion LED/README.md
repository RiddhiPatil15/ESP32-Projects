<h2>Motion LED</h2>
This Arduino project controls an LED based on motion detection using a digital motion sensor connected to pin 25. 
The LED is turned on when motion is detected and turned off otherwise.<br>

<h3>Components</h3>
1x Arduino board (e.g., ESP32)<br>
1x Motion sensor connected to pin 25<br>
1x LED connected to pin 18<br>
Jumper wires<br>
Breadboard (optional)<br>

<h3>Working</h3>
The motion sensor is connected to pin 25 and read using digitalRead().<br>
If motion is detected (motion == HIGH), the LED connected to pin 18 is turned on.<br>
If no motion is detected, the LED stays off.<br>
The sensor readings are also printed to the serial monitor for debugging purposes.<br>

<h3>Code Explanation</h3>
<h4>void setup()</h4>
Initializes the serial communication at a baud rate of 115200.<br>
Configures pin 25 as input for the motion sensor.<br>
Configures pin 18 as output for the LED.<br>
<h4>void loop()</h4>
Reads the motion sensor value from pin 25.<br>
Prints the sensor value to the serial monitor.<br>
If motion is detected, the LED is turned on; otherwise, it remains off.<br>
A short delay (delay(10)) is used to smooth out the readings.<br>

<h3>Circuit Diagram Connections</h3>
Pin 25: Connected to the motion sensor's output pin.<br>
Pin 18: Connected to the positive leg of the LED (with a suitable resistor in series).<br>
