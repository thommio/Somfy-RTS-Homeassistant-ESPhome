# Somfy-RTS-Homeassistant-ESPhome
Control your somfy blinds with homeassistant with the help of ESPhome

Connect an 433mhz transmitter to GPIO4 of the ESP32. Make sure you change the crystal for a 433.4mhz one. If you don't do this it might work but reception will be bad
![image](https://user-images.githubusercontent.com/82468260/224290841-80bbd43d-1937-4859-889f-cb252a0aedb9.png)


copy somfy_secrets.h and somfy_cover.h the directory "/esphome" 

Make a new device in esphome and use 'somy.yaml'


To program it you need a working remote. 
- go to somfy.local or the local Ip adress of the esp32, for me this is 192.168.1.196
- Grab your working somfy remote, choose the channel of the blind you want to program
- press an hold the program button on the back of the remote until the blind goes up and down.
- press the prog. button on the esp32, the blind should move shortly up and down again.
- That's it!

- known bug: Codes seems to reset when you reboot the esp32. Reprogramming it doesnst seen to work after this. 
You wil have to change the remoteadresses in "somfy_secrets.h". 

