# IOT-Smart-Home System
This project is an IoT-based Smart Home System designed to monitor environmental conditions and control devices. It uses an ESP8266 E12 microcontroller, a DHT11 sensor, ultrasonic sensor, LEDs, and a buzzer to perform edge computing and communicate with ThingSpeak for data logging and analysis.

Features <br>
Environmental Monitoring: Measures temperature and humidity using a DHT11 sensor.
Distance Measurement: Uses an ultrasonic sensor to detect obstacles and measure distance.
Alert System: Includes an LED and buzzer for notifications based on threshold values.
Data Logging: Sends sensor data to ThingSpeak for real-time monitoring and visualization.
WiFi Connectivity: Connects to a WiFi network for data communication.

Hardware Components <br>
ESP8266 microcontroller
DHT11 Temperature and Humidity Sensor
Ultrasonic Sensor (HC-SR04)
LEDs (Red, Green, Blue, Alert)
Buzzer
Miscellaneous: Breadboard, resistors, wires

Software Requirements <br>
Arduino IDE
ESP8266 WiFi Library
ThingSpeak Library
DHT Library

Circuit Setup<br>
Connect the DHT11 sensor to the ESP8266 as follows:
Data pin to GPIO2 (D4)
Power and Ground to VCC and GND
Connect the ultrasonic sensor:
Trig pin to GPIO14 (D5)
Echo pin to GPIO12 (D6)
Connect the LEDs:
Red LED to GPIO5 (D1)
Green LED to GPIO4 (D2)
Blue LED to GPIO0 (D3)
Alert LED to GPIO15 (D8)
Connect the buzzer to GPIO13 (D7).

Configuration<br>
Update WiFi credentials and Thingspeak configurations in the code:

Usage<br>
Power on the ESP8266 module.
The system will connect to the specified WiFi network.
Sensor readings are displayed on the serial monitor and sent to ThingSpeak.
Alerts are triggered when values exceed predefined thresholds.

Edge Computing<br>
Implements smoothing algorithms to average sensor readings.
Maintains a rolling buffer for efficient data processing.

Future Improvements<br>
Integration with a mobile app for remote monitoring.
Voice control using Google Assistant or Alexa.
Expandable support for additional sensors or devices.
