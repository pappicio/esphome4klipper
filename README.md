# esphome4klipper

project to connect esphome relay module to power.ON/OFF, emergency shutdown 3D printer running klipper

you need: esp32/esp8266 (at moment ESP32 S2 is used!), a relay module (2 relay module at moment), a (110/220V) micro powersupply, a case and 2 push buttons (3 push button at moment)

you need connect wires to your esp32 (at moment ESP32 S2):

pin: GPIO40
id: led status 3d printer
    
pin: GPIO38
id: multi plug state led

pin: GPIO34
id: 3d printer relay

pin: GPIO36
id: multiplug relay

GPIO39 shudown 3d printer-emergency push button

GPIO35 turn ON/OFF safety 3d printer push button

GPIO37 multiplug turn ON/OFF push Button

and 220V to power supply and from its output 5v to esp32 GPIO: 5V and GND

flash esphome on ESP32 and copy/paste or add config files on klipper files, restart 3D printer and you're ON!

P.S.: Added a multi-plug for different uses!!!!, so 2 relays, one for 3D- printer, other for multi-plug...
