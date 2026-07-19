# ESP-NOW Wireless Vision RC Car

This is the whole codebase for my espnow vision car it hass all the cad files of car and reemote and all the code to create your own simply also this car is not like any other car on youtube it actually uses esp32 cam to display the vision on the remote and also has joystick speed controls.

The reason I built this is like firstly an rc car is a very commen project so i thought i might be cool to create some thing very unique out of this common thing like a physical remote with joystick then a camera with on remote live feed is very very unique like i searched many yt videos still havent found a single one also another reason was esp-now protocol i have not used it any time so it was a nice time to try some thing new for me also.

[For stp files https://drive.google.com/drive/folders/1rErOXvgO1o4XdKNtQUgpyoMaxtlu1l8J?usp=sharing]


## Features

- Peer-to-peer communication using ESP-NOW
- No Wi-Fi router or internet required
- Low-latency wireless data transfer
- Easy to understand and modify
- Suitable for robot control and sensor communication
- Live vison on remote
  
## BOM-Bill Of Materials
| Component               |   Quantity  | Description                                                     |
| ----------------------- | :---------: | --------------------------------------------------------------- |
| ESP32 Development Board |      3      | One transmitter and one receiver                                |
| TB6612FNG Motor Driver  |      1      | Dual H-Bridge motor driver                                      |
| TT Dual Shaft DC Motor  |      4      | Geared DC motors for robot movement                             |
| 65 mm Wheels            |      4      | Compatible with TT motors                                       |
| ESP32-CAM               |      1      | Wireless camera module                                          |
| 1.8" TFT Display        |      1      | Display for remote interface                                    |
| LM2596 Buck Converter   |      1      | Voltage regulation                                              |
| 18650 Li-ion Battery    |      2      | Power source                                                    |
| 18650 Battery Holder    |      1      | Battery mounting                                                |
| 3D Printed Parts        | As required | Motor mounts, camera mount, brackets, remote enclosure, spacers |
| Screws, Nuts & Spacers  | As required | Mechanical assembly                                             |
| Jumper Wires            | As required | Electrical connections                                          |

<img width="4032" height="3024" alt="WhatsApp Image 2026-01-04 at 19 02 38 (1)" src="https://github.com/user-attachments/assets/40689f4f-7b3a-48da-b1aa-4144226c5746" />

Circuit Diagrams(for clear circuit diagram visit :https://app.cirkitdesigner.com/project/403f83fd-756a-48fe-b7f0-dc32b4001005)
Car-
<img width="460" height="323" alt="Screenshot 2026-07-14 at 6 38 22 PM" src="https://github.com/user-attachments/assets/fe6b1260-42a8-4b52-95f0-b99cc3efa059" />
Remote-
<img width="339" height="248" alt="Screenshot 2026-07-14 at 6 39 58 PM" src="https://github.com/user-attachments/assets/0f11cd60-92a7-4913-a580-39ca332b2b31" />

Camera-
<img width="3534" height="3705" alt=" connection" src="https://github.com/user-attachments/assets/aa056e94-5c6c-4033-9dcb-c37865f584fc" />
