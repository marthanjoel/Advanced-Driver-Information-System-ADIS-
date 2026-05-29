# Advanced Driver Information System (ADIS)

## Overview

This project is an Advanced Driver Information System (ADIS) built using Arduino Uno.

The system simulates a smart vehicle dashboard capable of:

* displaying real-time date and time
* monitoring temperature
* monitoring fluid levels
* providing visual and sound warnings

The project demonstrates embedded systems integration using sensors, displays, warning systems, and real-time monitoring.

---

# Features

## LCD Dashboard Display

The LCD1602 with I2C displays:

* Date
* Time
* Temperature
* Warning messages

---

## Real-Time Clock (RTC)

The DS1302 RTC module keeps accurate date and time information even when the Arduino is powered off.

---

## Temperature Monitoring

The LM35 temperature sensor measures system temperature.

### Temperature Status

| Temperature    | Status  | RGB Color |
| -------------- | ------- | --------- |
| Below 30°C     | Normal  | Green     |
| 30°C – 39°C    | Warning | Blue      |
| 40°C and above | Danger  | Red       |

---

## Water/Fluid Monitoring

The water sensor simulates monitoring vehicle wiper fluid levels.

When the fluid level becomes low:

* LCD warning appears
* RGB LED turns red
* Buzzer alert activates

---

## RGB Warning System

The RGB LED provides system status indication.

| Color | Meaning   |
| ----- | --------- |
| Green | System OK |
| Blue  | Warning   |
| Red   | Danger    |

---

## Buzzer Alerts

The buzzer provides audible warnings during dangerous conditions.

---

# Components Used

* Arduino Uno
* LCD1602 with I2C
* DS1302 RTC module
* LM35 temperature sensor
* Water level sensor
* RGB LED (Common Cathode)
* Active buzzer
* Breadboard
* Jumper wires
* 220Ω resistors

---

# Wiring Connections

## LCD1602 I2C

| LCD Pin | Arduino Uno |
| ------- | ----------- |
| GND     | GND         |
| VCC     | 5V          |
| SDA     | A4          |
| SCL     | A5          |

---

## RTC DS1302

| RTC Pin | Arduino Uno |
| ------- | ----------- |
| DAT     | D4          |
| CLK     | D6          |
| RST     | D5          |
| VCC     | 5V          |
| GND     | GND         |

---

## LM35 Temperature Sensor

| LM35 Pin | Arduino Uno |
| -------- | ----------- |
| Left     | 5V          |
| Middle   | A0          |
| Right    | GND         |

---

## Water Sensor

| Water Sensor | Arduino Uno |
| ------------ | ----------- |
| S            | A1          |
| +            | 5V          |
| -            | GND         |

---

## RGB LED

| RGB Pin        | Arduino Uno |
| -------------- | ----------- |
| Red            | D10         |
| Green          | D11         |
| Blue           | D9          |
| Common Cathode | GND         |

---

## Buzzer

| Buzzer Pin | Arduino Uno |
| ---------- | ----------- |
| +          | D8          |
| -          | GND         |

---

# Software Used

* Arduino IDE
* C++ / Arduino Programming Language

---

# How the System Works

1. The RTC module provides real-time date and time.
2. The LM35 sensor measures temperature.
3. The water sensor monitors fluid level.
4. The LCD displays system information.
5. The RGB LED changes color depending on system condition.
6. The buzzer activates during warning or danger conditions.

---

# Future Improvements

Future versions of the system can include:

* 8x8 LED Matrix warning symbols
* 7-segment odometer display
* Sound sensor for voice control
* Multiple temperature sensors
* OBD-II vehicle integration
* Speed and RPM monitoring

---

# Project Purpose

This project was developed for learning and demonstrating:

* Embedded systems
* Sensor interfacing
* Real-time monitoring systems
* Vehicle dashboard simulation
* Arduino programming

---

# Author

Lutwama Joel Marthan

---

# License

This project is open for educational and learning purposes.



