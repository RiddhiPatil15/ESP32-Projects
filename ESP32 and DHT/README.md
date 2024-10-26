<h2>ESP32 & DHT</h2>
This project uses an ESP32 microcontroller with a DHT11 sensor to measure and display real-time temperature and humidity on a web server.<br>
The ESP32 connects to a Wi-Fi network and hosts a web page accessible via the device’s IP address, where users can view the sensor data in a browser.

<h3>Components</h3>
ESP32 Microcontroller<br>
DHT11 Sensor (Temperature and Humidity)<br>
Wi-Fi Network<br>

<h3>Prerequisites</h3>
Arduino IDE: Ensure it’s installed on your computer.<br>
ESP32 Board Package: Configure ESP32 board settings in Arduino IDE.<br>
DHT Library: Install DHT sensor library by Adafruit through the Arduino Library Manager.<br>

<h3>Project Setup</h3>
<h5>Wiring:</h5>
Connect the DHT11 sensor’s data pin to GPIO12 on the ESP32.<br>
Connect VCC and GND to the ESP32’s 3.3V and GND pins.<br>
<h5>Code Setup:</h5>
Update the ssid and pwd variables with your Wi-Fi network's SSID and password.<br>
Adjust the baud rate if needed.<br>

<h3>Code Walkthrough</h3>
WiFi Connection: Connects the ESP32 to the specified Wi-Fi network and displays the IP address.<br>
DHT Sensor: Reads temperature and humidity values from the DHT11 sensor.<br>
Web Server: Hosts a web page on port 80, displaying the sensor data in HTML format.<br>

<h3>How to Use</h3>
Upload the Code: Upload the code to your ESP32 via the Arduino IDE.<br>
Connect to Wi-Fi: The Serial Monitor will display the connection status. Once connected, note the IP address.<br>
Access Web Page: Open a browser and enter the IP address (e.g., http://192.168.1.xx/) to view the temperature and humidity data.<br>
