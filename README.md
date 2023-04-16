# creamlity-CR-10-Firmware-Marlin
A Full MarlinFirmware for the creality CR-10 Printer for everybody who doesn't like to configure anything.

Made for the Creality V1 mainboard with a ATmega1284P controler


# What you need for Flash with new bootloader

1. VScode with "marlin firmware Auto Build" and "PlatformIO IDE"
2. https://github.com/Lauszus/Sanguino
3. Arduino uno
4. 6 male to female jumper cables


# What you need for FLash without new bootloader

1. VScode with "marlin firmware Auto Build" and "PlatformIO IDE"

# Flash with new bootloader

1. connect pin 1 (MISO) to pin 12, pin 2 (VCC) to +5V, pin 3 (SCK) to pin 13, pin 4 (MOSI) to pin 11, pin 5 (RST) to pin 10, pin 6 (GND) to GND on your Arduino
2. Open The Arduion IDE
3. Open File/Examples/11.ArduinoISP/ArduinoISP
4. upload the sketch to your Arduino
5. power on your printer an check if everything is connected correctly
6. enable /Tools/Board/Sanguion-avr/Sangoino
7. enable /Tools/Processor/ATmega1284 or ATmega1284P (16Mhz)
8. pick the right port /Tools/Port
9. change the bootloader /Tools/Programmer/Arduino as ISP
10. click /Tools/Burn Bootloader
11. check if there are no errors
12. unplug everything, you now only need your 3d Printer
13. swich the only jumper on the board to the USB state
14. plug in your board again / turn on your printer
15. Open the Marlin folder with the "Marlin Firmware" plugin in VScode
16. in case the ABM pannes doesnt pop up, open it by clicking "show ABM Panel" in the "Auto build Marlin" Menu
17. Click on the Build butten next to "melzi_optiboot_optimized"
18. wait for the build to complete
19. check for errors
20. after completing click on the upload butten
21. wait for the upload to complete
22. check for errors
23. change the jumper back in the original state

Finished!

#Flash without new bootloader

1.swich the only jumper on the board to the USB state
2. plug in your board again / turn on your printer
3. Open the Marlin folder with the "Marlin Firmware" plugin in VScode
4. in case the ABM pannes doesnt pop up, open it by clicking "show ABM Panel" in the "Auto build Marlin" Menu
5. Click on the Build butten next to "melzi_optiboot_optimized"
6. wait for the build to complete
7. check for errors
8. after completing click on the upload butten
9. wait for the upload to complete
10. check for errors
11. change the jumper back in the original state

Finished!
