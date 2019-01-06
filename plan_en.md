 # Manual - node ttn-tul-node-v1
 
 ## Arduino configuration
 ### Download Arduino IDE
 Links to the software is available on the website: https://www.arduino.cc/en/Main/Software.
 ### Test the Arduino Board 
 The easiest way to test the Arduino board is to load "Blink" example.
 You can find the project in the menu File/Examples/01.Basics/Blink or go throught tutorial: https://www.arduino.cc/en/Tutorial/Blink.
 ### Install the LMIC-Arduino library 
 Go to Sketch/Include Library\Manage Libraries... and search for "LMIC-Arduino". Install the newest version.
 ## Portal thethingsnetwork.com
 ### Zarejestrowac się
 ### Utworzyć nową apliakcję oraz czujnik
 ## Uzyskać dane do portalu PŁ "LoraStore"
 ## Arduino + LoRa
 ### Uruchomić sample ttn-abp z biblioteki LMIC-Arduino
 ### Podpiąć pod arduino tt-tul-node-v1 board z rfm95w oraz 1 dowolnym czujnikiem
 ### Uruchomić czujnik, wartośc odczytu z czujnika wykorzystac dalej gdy będzie potrzebna zmienna value
 ### Podmienić dane dotyczące sieci:
 			i. NWKSKEY
 			ii. APPSKEY
 			iii. DEVADDR
 ### Zamienić domyślną wysyłaną wiadomość "Hello World" na Jsona zawierającego:
 			i. SensorId (String)
 			ii. SensorPassword (String)
 			iii. Value (zmienna real)
 ## Testowanie działania programu
 ### Spawdzić na stronie console ttn czy widac ze dane przechodzą przez portal
 ### Sprawdzić czy endpoint logguje wyniki: https://lorastore20181206101456.azurewebsites.net/api/Measurements?id=3 (gdzie id to numer SensorId)
