# ESP-NOW Wireless Vision RC Car

This is the whole codebase for my espnow vision car it hass all the cad files of car and reemote and all the code to create your own simply also this car is not like any other car on youtube it actually uses esp32 cam to display the vision on the remote and also has joystick speed controls.

The reason I built this is like firstly an rc car is a very commen project so i thought i might be cool to create some thing very unique out of this common thing like a physical remote with joystick then a camera with on remote live feed is very very unique like i searched many yt videos still havent found a single one also another reason was esp-now protocol i have not used it any time so it was a nice time to try some thing new for me also.

[For stp files https://drive.google.com/drive/folders/1rErOXvgO1o4XdKNtQUgpyoMaxtlu1l8J?usp=sharing]


## Features

- Peer-to-peer communication using ESP-NOW
- No Wi-Fi router or internet required fully offlinee
- Low-latency wireless data transfer
- Easy to understand and modify
- Suitable for robot control and sensor communication
- Live vison on remote
  

## BOM – Bill of Materials

| Component | Quantity | Price | Purpose | Purchase Link |
|-----------|:--------:|:-----:|---------|:-------------:|
| ESP32 Dev Board | 3 | $3.96/pc | Wireless communication | [Buy Here](https://robu.in/product/esp-wroom-32-wifi-bluetooth-networking-smart-component-development-board/) |
| TB6612FNG Motor Driver | 1 | $1.45 | Drive DC motors | [Buy Here](https://robu.in/product/motor-driver-tb6612fng-module-performance-ultra-small-volume-3-pi-matching-performance-ultra-l298n/) |
| TT Dual Shaft DC Motor | 4 | $1.27/pc | Locomotion | [Buy Here](https://robu.in/product/230rpm-straight-type-dual-side-6v-bo-motor/) |
| 65 mm Wheels | 4 | $0.25/pc | Mobility | [Buy Here](https://robu.in/product/robot-smart-car-wheel-tyre-bo-motor/) |
| 18650 Li-ion Battery | 3 | $1.45/pc | Power source | [Buy Here](https://robocraze.com/products/18650-2200mah-3-7v-battery-cylinder-type-blue?variant=43800370249952) |
| 18650 Battery Holder | 1 | $0.26 | Battery mounting | [Buy Here](https://robu.in/product/black-plastic-storage-box-case-holder-battery-3-x-18650-cell-box-without-cover/) |
| LM2596S Buck Converter | 1 | $0.44 | Voltage regulation | [Buy Here](https://robu.in/product/lm2596s-dc-dc-buck-converter-power-supply/) |
| ESP32-CAM | 1 | $6.60 | Vision module | [Buy Here](https://robocraze.com/products/esp32-camera-module?variant=40193645707417) |
| ESP32-CAM MB *(Optional)* | 1 | $1.14 | USB programmer for ESP32-CAM | [Buy Here](https://techtonics.in/product/esp32-cam-mb-micro-usb-download-module-for-esp32-cam-development-board/) |
| 1.8" TFT Display | 1 | $4.16 | User interface | [Buy Here](https://robu.in/product/goldenmorning-1-8-inch-tft-module-128x160-st7735s/) |
| Screws, Nuts & Spacers | As required | $4–$5 | Mechanical assembly | Local Hardware Store |
| 3D Printed Parts | 12 | Self-manufactured | Structural support and mounts | Self Printed |


<img width="4032" height="3024" alt="WhatsApp Image 2026-01-04 at 19 02 38 (1)" src="https://github.com/user-attachments/assets/40689f4f-7b3a-48da-b1aa-4144226c5746" />

Circuit Diagrams(for clear circuit diagram visit :https://app.cirkitdesigner.com/project/403f83fd-756a-48fe-b7f0-dc32b4001005)
Car-
<img width="460" height="323" alt="Screenshot 2026-07-14 at 6 38 22 PM" src="https://github.com/user-attachments/assets/fe6b1260-42a8-4b52-95f0-b99cc3efa059" />
Remote-
<img width="339" height="248" alt="Screenshot 2026-07-14 at 6 39 58 PM" src="https://github.com/user-attachments/assets/0f11cd60-92a7-4913-a580-39ca332b2b31" />

Camera-
<img width="3534" height="3705" alt=" connection" src="https://github.com/user-attachments/assets/aa056e94-5c6c-4033-9dcb-c37865f584fc" />


## How to Build this...
I had uploaded all the needed code , cad models and complete circuit diagram in my repo 

step 1: first in code folder get the mac address upload that code in the esp that will be in your main car on uploading go to serial moniter press the rst button on esp once you will get its mac address copy it some where.

step 2: It is optional but I would recommend to do it to check once the values of your joystick just connect the joystick to the esp as in the diagram in 34 and 35 and then just upload the code and check the values if u are getti.ng values great other wise there might be something wrong in joystick or esp

step 3: get the esp for your remote and the mac address now mac address will be something like this 48:e7:29:b2:e6:3c u need to convert it into this 0x48, 0xE7, 0x29, 0xB2, 0xE6, 0x3C just separate each and add 0x in front now change mac address acc to yours in the transmitter coade and hit upload

step 4: Upload your car esp with the reciever code and voila your remote control car is done 

step 5: Now for vision just upload the esp32cam code in the esp32 cam with a cam mb or ftdi up to you

step 6: this is very much complicated and i personally spend too much time on it first download TFT_eSPI library now go to your arduino folder then library then search for tft espi and inside that u will get something named User_Setup.h now u need to modify it according to your display firstly everythings thats in there and replace with my user setup file now go to line 45 i had a ili9342 display so i used that which ever driver your display has just uncomment that driver and comment the rest ok if you dont know the driver just check each and every one once done upload the espcam_display code and done your cam and display works now

step 7 : It was the mst annoying for me not for you actually to get the car for optinal speed and work smoothly every thing needs to balance out so i had to arrange all the items in very specific manner so weight is equally distributed so for assembly i had uploaded stp and f3z files so just check my placements u need to do some solderings and then just screw them into place and it will be done also the top part is just open space so if you have any figurine or any model u can attach there like i attached a robotic arm on top of it from my previous projects

step
