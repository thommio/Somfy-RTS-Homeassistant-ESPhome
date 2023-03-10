# Somfy-RTS-Homeassistant-ESPhome
Control your somfy blinds with homeassistant with the help of ESPhome

Connect an 433mhz transmitter to GPIO4 of the ESP32. Make sure you change the crystal for a 433.4mhz one. If you don't do this it might work but reception will be bad
![image](https://user-images.githubusercontent.com/82468260/224290841-80bbd43d-1937-4859-889f-cb252a0aedb9.png)


copy somfy_secrets.h and somfy_cover.h the directory "/esphome" 

Make a new device in esphome and use 'somy.yaml'
