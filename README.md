# LXESP32DMX

## Modified by MGR: 
- forked from 02/03/2020 f2466dde9a0879c75164c432dc0333f82cbabeb4
- add uart config for RX
- Tested with Arduino IDE 1.8.13 // esp32 board manager v1.0.6 // MH ET LIVE DevKit


## LX README:
DMX Driver for ESP32 using ArduinoIDE and Arduino core for the ESP32.

Driver outputs DMX using UART2 on GPIO pin 17.

Driver inputs DMX using UART2 with modified hardware abstraction file on GPIO pin 16.

Arduino core for the ESP32 is found at https://github.com/espressif/arduino-esp32

Install Arduino core for the ESP32 into [path to sketch folder]/Arduino/hardware/.

Replace the following file:

[path to sketch folder]/Arduino/hardware/espressif/esp32/cores/esp32/esp32-hal-uart.c

with the file included with this library in the extras/modified_hal-uart folder.
