# ESPHome-Presence-Detector_With-PCB
I was tired of my lights constantly turning off whenever I sat still while using a standard PIR motion detector. Since PIR sensors only detect "big movements", they often fail to notice someone who is sitting quietly.

To solve this, I built a presence detector using an mmWave sensor. Unlike a traditional PIR sensor, an mmWave sensor can detect very small movements, such as your chest moving while breathing, allowing it to reliably detect occupancy even when you're not moving around.

While designing the project, I decided to add a few extra features:

* **mmWave presence detection** for reliable occupancy sensing
* **PIR motion sensor** for fast motion detection when entering the room
* **Ambient light sensor** to prevent lights from turning on when the room is already bright
* **Status LED** to indicate Wi-Fi or device issues
* **Custom PCB** to keep the wiring clean and make assembly easier

The PCB connects all modules directly to the microcontroller, making installation as simple as plugging the sensors into their designated headers.

Sensor data is sent to Home Assistant using ESPHome, allowing you to create virtually any automation you can think of —from automatically controlling lights to sending notifications when someone enters a room, everything is possible.

## Requirements

Before starting this project, you will need:

1. A working Home Assistant server
2. A soldering iron and basic soldering skills
3. A bit of patience and a good mood ;)

**Note:** The status LED and its resistor are small and can be quite challenging to solder. If you don't care about the LED, it can be left out.

## PCB Design

schematic:
<img width="492" height="559" alt="image" src="https://github.com/user-attachments/assets/635c814a-1ec2-460c-b19b-519687a2a4ce" />

PCB:
<img width="169" height="261" alt="image" src="https://github.com/user-attachments/assets/f12dec24-2f32-47f8-8688-a15900c4763b" />

## Design Inspiration

I wanted a clean and modern design for the detector, so i kindly asked chatGPT to make a few diffrent designes and shapes before settling on this final version:

<img width="1408" height="768" alt="Gemini_Generated_Image_1y6acm1y6acm1y6a" src="https://github.com/user-attachments/assets/b65594e3-b6e7-40ee-b4ca-89776852eb45" />

i then started modeling my own...
<img width="1279" height="720" alt="image" src="https://github.com/user-attachments/assets/5e05eeb4-a0a9-40d9-826e-b2632748764f" />


## Project Status

🚧 This project is still under development.

Additional documentation will be added soon, including:

* Complete assembly guide
* ESPHome configuration- and firmware instalation guide
* refined 3D-printable enclosure files

Thank you for your patience while I finish building and documenting the project.






BOM:
1. ws2812b LED
   <img width="668" height="632" alt="image" src="https://github.com/user-attachments/assets/1b975414-5dca-4ebe-80f4-aab977681654" />

2. TSL2591 IIC I2C Light Sensor
   <img width="464" height="386" alt="image" src="https://github.com/user-attachments/assets/b0bf1e9d-2cc1-491a-8073-a0734676d4b0" />

3. ESP32 S3 C3 SuperMini Development Board
   <img width="444" height="399" alt="image" src="https://github.com/user-attachments/assets/3a2f3fb9-ce43-4df6-8553-18630505c2fb" />

5. HLK-LD2410c module
   <img width="357" height="411" alt="image" src="https://github.com/user-attachments/assets/631f1854-0919-49bc-8c19-3cfc71566e63" />

7. AM312 PIR motion detector
   <img width="378" height="380" alt="image" src="https://github.com/user-attachments/assets/1dea22d9-4476-4875-b6ef-096d0a11617e" />

8. Female Straight Needle Pin Header
   <img width="453" height="299" alt="image" src="https://github.com/user-attachments/assets/f0fa145c-1d12-4137-880b-a00f2f7623d5" />

9. Custom PCB (gerber files are linked in the project)
    <img width="507" height="772" alt="image" src="https://github.com/user-attachments/assets/1ea670e9-7abb-478a-92b8-1a5198646aa3" />

    
