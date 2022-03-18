# ESP8266 with OLED, DHT11, GY-30 and BMP180
My fourth trying with Arduino and show lux data on a mini OLED display.<br>
Its display my text who made this code and after that its will shows the data.

## Parts: 
- Adafruit ESP8266 as NodeMCU 1.0 (ESP-12E modul),
- 0.96″ 128x64 mini OLED display (I use white color for that project),
- DHT11 temperature and humidity sensor
- GY-30 Light Intensity Sensor
- BMP180 Air Pressure Sensor
- Jumper cables.


You can see a picture from the full setup here:<br>
![Picture from the setup](/ESP8266-OLED-DHT11-GY30-BHP180.jpg)

## Arduino Modules:
- Adafruit_SSD1306,
- Adafruit_GFX,
- DHT
- BH1750 for the GY-30
- SFE_BMP180 for the BMP180 Air Pressure Sensor

It is the next step on my previous project as ![ESP8266 with DHT11, GY-30 and OLED](https://github.com/Mategm/ESP8266-DHT11-GY30-OLED)<br>

## Connection:
- Display GND to ESP G (Ground beside the 3V)
- Display VCC to ESP 3V
- Display SCL to ESP D1 as GPIO 1
- Display SDA to ESP D2 as GPIO 2
- DHT + to ESP 3V (Can be the same as where the display VCC)
- DHT - to ESP G (Can be the same as where the display GND)
- DHT OUT to ESO D5 as GPIO 14
- GY-30 VCC to ESP 3V (Can be the same as where the display VCC)
- GY-30 GND to ESP G (Can be the same as where the display GND)
- GY-30 SCL to ESP D1 as GPIO 1 (Can be the same as where the display SCL)
- GY-30 SDA to ESP D2 as GPIO 2 (Can be the same as where the display SDA)
- BMP180 VIN to ESP 3V (Can be the same as where the display VCC)
- BMP180 GND to ESP G (Can be the same as where the display GND)
- BMP180 SCL to ESP D1 as GPIO 1 (Can be the same as where the display SCL)
- BMP180 SDA to ESP D2 as GPIO 2 (Can be the same as where the display SDA)


Coding in Arduino IDE 1.8.19<br>
I made this code from sources of the internet. There is no copyright, use it as you want.
