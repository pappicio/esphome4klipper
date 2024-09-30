# esphome4klipper

project to connect esphome relay module to power.ON/OFF, emergency shutdown 3D printer running klipper

you need: esp32/esp8266, a relay module, a (110/220V25V) micro poersupply, a case and 2 push buttons

you need connect wires to your esp32:


GPIO2 and gnd to push button1

GPIO3 and gnd to push button2

GPIO4 to pilote relay module

and 220V to power supply and from its output 5v to esp32 GPIO: 5V and GND

flash esphome on ESP32 and copy/paste or add config files on klipper files, restart 3D printer and you're ON!
