 # Manual - node ttn-tul-node-v1
 
 ## Arduino configuration
 ### Download Arduino IDE
 Link to the software is available on the website: https://www.arduino.cc/en/Main/Software.
 ### Test the Arduino Board 
 The easiest way to test the Arduino board is to load the "Blink" example.
 You can find the project in the menu File/Examples/01.Basics/Blink or go throught tutorial: https://www.arduino.cc/en/Tutorial/Blink.
 ### Install the LMIC-Arduino library 
 Go to Sketch/Include Library\Manage Libraries... and search for "LMIC-Arduino". Install the newest version.
 ## thethingsnetwork.com portal
 ### Sign up or login if you have account
 ### Create new application and sensor
 ## Uzyskać dane do portalu PŁ "LoraStore"
 ## Arduino + LoRa
 ### Open example "ttn-abp" from LMIC-Arduino library
 ### Connect 1 sensor and tt-tul-node-v1 board with rfm95w to Arduino
 ### Turn on the sensor and get the measurement. It will be used to modify the variable "value".
 ### Replace following network data:
 			i. NWKSKEY
 			ii. APPSKEY
 			iii. DEVADDR
 ### Replace default "Hello World" message with Json, which contains:
 			i. SensorId (String)
 			ii. SensorPassword (String)
 			iii. Value (zmienna real)
 ## Testing program
 ### Check on the console ttn website if data go throught the portal.
 ### Check if the endpoint is logging data: https://lorastore20181206101456.azurewebsites.net/api/Measurements?id=3 (Id is SensorId)
