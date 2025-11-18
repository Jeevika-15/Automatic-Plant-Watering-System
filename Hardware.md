*Components*
1.ESP32 development board
2.Soil moisture sensor 
3.Relay module (5V)
4.Mini water pump
5.External power supply for pump
6.Jumper wires

*Circuit Connection*
1. Soil Moisture sensor
   Sensor VCC → ESP32 3.3V
   Sensor GND → ESP32 GND
   Sensor AO → ESP32 GPIO 34

2. Relay Module
   Relay VCC → ESP32 5V
   Relay GND → ESP32 GND
   Relay IN → ESP32 GPIO 25

3. Water Pump
   Pump positive terminal → Relay NO (Normally Open)
   Relay COM → External power supply positive terminal
   Pump negative terminal → External power supply negative terminal

*Operation*
The moisture sensor sends an analog value to the ESP32. When moisture drops below the set threshold, the ESP32 outputs HIGH to the relay module, switching the pump on. Once the soil becomes moist, the output goes LOW and the pump turns off.![hardware2](https://github.com/user-attachments/assets/93434322-1005-426f-9ead-4d090b16d8e1)
![hardware1](https://github.com/user-attachments/assets/a4e9da8b-4785-4053-b65a-739ff6aaea79)
![hardware2](https://github.com/user-attachments/assets/aa4f7140-eb4e-494d-8549-10ff95b0f04c)
