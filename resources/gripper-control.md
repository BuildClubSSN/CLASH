# Gripper Assembly Division

## Introduction
The gripper is like the 💪**hand**, responsible for detecting, picking, and placing cubes.
- A 2-DOF(Degrees Of Freedom) gripper that is capable of lifting a cube of dimensions 5x5x5 cm weighing 50 g is required to be built and assembled along with a color sensor and proximity sensor. 
- The color sensor detects the color of the cube by reading the strip that is to be placed opposite to the cube position (on the right), while the proximity sensor has to detect the presence of the cube placed at the left of the track within a fixed distance of about 15 cm. 
- The proximity sensor ensures there's a cube present and the reading isn't a false positive and also acts as a fail safe mechanism to detect if the arm has lifted the cube up. 
- The position of the sensors are to be strategically decided upon by each of the teams. - The gripper, color sensor and proximity sensor extensions are exempt from the 20 x 20 x 20 cm dimension rule.


---

## Why this system is required
- Enables the bot to **interact physically with cubes**, not just navigate.  
- Ensures cubes are **securely gripped and lifted** without slipping.  
- Detects **cube presence** before attempting a lift (fail-safe).  
- Identifies cube **color** for placement in correct zones.    

---

## How it works
- The **gripper uses 2 degrees of freedom (2-DOF)**:  
  - One servo for opening/closing the jaws.  
  - Another servo for lifting the cube up and down.  
- **Proximity sensor** (IR / Ultrasonic / Sharp IR):  
  - Detects if a cube is present within ~10 cm.  
  - Double-checks whether the cube has been lifted (fail-safe).  
- **Color sensor** (TCS3200 / TCS34725):  
  - Reads the color strip opposite to the cube position. 
  - Sends the color information to the microcontroller.
- The combined system ensures **sense → verify → lift → place** in a reliable sequence.  

---

## Common options

### Actuators
- **SG90 Servo Motor** – lightweight, affordable, good for light tasks.  
- **MG90 Servo Motor** – metal gear, more durable, better torque (recommended).  

### Proximity Sensors
- **IR Sensor** – simple, cost-effective for close range.  
- **Ultrasonic Sensor** – accurate distance measurement, but bulkier.  
- **Sharp IR Sensor** – compact, good analog distance reading.  

### Color Sensors
- **TCS3200 / GY-31** – widely available, frequency output.  
- **TCS34725** – more accurate, I²C interface, good color sensitivity.  

### Gripper Mechanism
- **Prebuilt gripper kits** (MG90 compatible).  
- **DIY gripper (ice-cream stick method)** – cost-effective and customizable.  

---

## Useful resources
- [SG90 Servo Motor (Amazon)](https://www.amazon.in/Super-Debug-TowerPro-Rotation-Robotics/dp/B0827GB5DT)  
- [MG90 Servo Motor (Amazon)](https://www.amazon.in/Electrobot-MG90S-Vehicle-Helicopter-Models/dp/B08VMNX12X)  
- [IR Sensor Module (Amazon)](https://www.amazon.in/ApTechDeals-Infrared-Reflective-Photoelectric-Intensity/dp/B07Q1BSSFN)  
- [Ultrasonic Sensor (Amazon)](https://www.amazon.in/Banggood-Ultrasonic-Distance-Measuring-Transducer/dp/B01I1ZTPJC)  
- [Sharp IR Sensor (Amazon)](https://www.amazon.in/Robocraze-GP2Y0A21YK0F-Analog-Distance-10CM-80CM/dp/B07F6Y8HC9)  
- [TCS34725 Color Sensor (Amazon)](https://www.amazon.in/Techtonics-CJMCU-34725-TCS34725-Sensor-Development/dp/B0977MZZ8R)  
- [DIY Gripper with Ice-Cream Sticks (YouTube)](https://youtu.be/18I-mJZhTbw?si=eRbNrv_fJ-X6paz9)  
- [Prebuilt Gripper (Amazon)](https://amzn.in/d/5FETK1A)  

---
 
