<h2>ESP32 DHT Sensor Data Logging to ThingSpeak</h2>
This project reads temperature and humidity data using a DHT11 sensor connected to an ESP32 microcontroller and sends the data to ThingSpeak for cloud storage and analysis.<br>

![flowchart](https://github.com/user-attachments/assets/e2c9dc90-e4e8-4b35-8b2d-f8cb266f44c7)


<h3>Components Used</h3>
ESP32: Microcontroller with WiFi capability.<br>
DHT11 Sensor: Measures temperature and humidity.<br>
ThingSpeak: Online platform to store and analyze IoT data.<br>

<h3>Code Explanation</h3>
This code uses WiFi and HTTPClient libraries to connect the ESP32 to a WiFi network and send data to ThingSpeak. <br>
The DHT11 sensor reads temperature and humidity, which are logged to the serial monitor and uploaded to ThingSpeak every 20 cycles.<br>

<h3>Key Parts of the Code</h3>
WiFi Setup: Connects the ESP32 to a WiFi network using your SSID and password.<br>
DHT11 Initialization: Sets up the DHT11 sensor on the specified pin.<br>
Data Logging Loop: Reads temperature and humidity from the DHT11 sensor, displays them on the serial monitor, and sends them to ThingSpeak every 20 cycles.<br>

<h3>How to Use the Code</h3>
Install Libraries: Make sure to install the WiFi and HTTPClient libraries, and the DHT library if not already installed.<br>
Update WiFi Credentials: Replace SSID and PASS with your WiFi network name and password.<br>
Insert ThingSpeak API Key: Replace "YOUR API KEY" in the code with your ThingSpeak channel's write API key.<br>
Upload Code to ESP32: Upload the code to the ESP32 via Arduino IDE or another preferred environment.<br>
