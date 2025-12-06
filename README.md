IoT Electricity Energy Meter Using ESP32 and Blynk

This is a simple IoT-based energy meter using ESP32. It measures voltage, current, power, and energy (kWh) and shows the readings on a 16x2 LCD and the Blynk app.

Features

Measures Vrms, Irms, Power, and kWh

Real-time monitoring on Blynk app

Optional LCD display for local readings

Updates every 5 seconds

What You Need

ESP32 WiFi Module

SCT-013 Current Sensor (0-30A)

ZMPT101B AC Voltage Sensor

16x2 LCD (optional)

10K Potentiometer

Resistors: 10K x2, 100Ω x1

Capacitor 10uF x1

Breadboard and jumper wires

Connections

Current Sensor → GPIO34

Voltage Sensor → GPIO35

LCD pins → D13, D12, D14, D27, D26, D25 (optional)

VCC and GND of sensors → 5V and GND of ESP32

Make sure AC wires are connected safely when using sensors

Libraries You Need

EmonLib

Blynk

LiquidCrystal

How to Use

Connect your hardware as mentioned above

Open IoT_Energy_Meter.ino in Arduino IDE

Update your WiFi name, password, and Blynk Auth Token in the code

Upload the code to ESP32

Watch real-time data on the Blynk app or optional LCD

Quick Calibration

Voltage vCalibration 83.3

Current currCalibration 0.50

Change these if readings don’t match actual values

Blynk Virtual Pins

V0 → Voltage (Vrms)

V1 → Current (Irms)

V2 → Power (W)

V3 → Energy (kWh)