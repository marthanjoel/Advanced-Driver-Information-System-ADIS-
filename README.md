# Advanced-Driver-Information-System-ADIS- 🚗

📌**** Overview****
The Mini ADIS is an Arduino-based vehicle dashboard simulation system built using an Arduino Uno. It displays real-time vehicle data such as time, date, and temperature, and provides visual and audio alerts using RGB LEDs and a buzzer.


🔧 **Features**
🕒 Real-Time Clock (RTC DS1302)
🌡️ Temperature Monitoring (LM35 sensor)
📟 LCD Display (I2C 16x2)
🌈 RGB LED Status Indicator
🔊 Buzzer Warning System
⚡ Real-time system updates


**🧠 System Logic**
Temperature Range	Status	RGB Color	Buzzer
< 30°C	Normal	Green	OFF
30°C – 40°C	Warning	Yellow	Beep
> 40°C	Danger	Red	Continuous


**🔌 Components Used**
Arduino Uno
DS1302 RTC Module
LM35 Temperature Sensor
I2C LCD 16x2
RGB LED (Common Cathode)
Active Buzzer
Jumper wires & breadboard


**Wiring Summary**
LCD (I2C)
SDA → A4
SCL → A5

RTC (DS1302)
DAT → D4
CLK → D6
RST → D5
VCC → 5V
GND → GND

LM35
OUT → A0
VCC → 5V
GND → GND

RGB LED
Red → D10
Green → D11
Blue → D9

Buzzer
→ D8
→ GND


**💻 Code Functionality**
The system:

Reads real-time clock data from DS1302
Reads temperature from LM35
Displays data on LCD
Changes RGB LED color based on temperature
Activates buzzer for warnings


**🚀 How to Run**
Open Arduino IDE
Install required libraries:
LiquidCrystal_I2C
Rtc by Makuna
Upload the main .ino file to Arduino Uno
Open Serial Monitor (9600 baud)
Observe LCD output and system behavior


**⚠️ Important Notes**
RTC must have a CR2032 battery installed
Remove Rtc.SetDateTime(__DATE__, __TIME__) after first upload
Ensure RGB LED is common cathode
Check wiring carefully before powering

🎯 Project Outcome
This project simulates a simplified vehicle dashboard system similar to real automotive information systems used in modern cars.

👨‍💻 Author
 _**LUTWAMA JOEL MARTHAN**_

Developed using Arduino Uno for learning embedded systems, sensors, and real-time monitoring.
