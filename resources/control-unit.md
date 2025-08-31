# 🧠 Microcontroller (MCU)

### Why we require a microcontroller  
- The microcontroller is the **brain of the robot**. Just like the brain processes signals from eyes/ears and tells muscles what to do, the MCU processes sensor data and controls motors/grippers. 
- It processes sensor inputs, applies algorithms (like PID for line following), and sends control signals to actuators.  
- Without the MCU, sensors and actuators would work in isolation with no coordination.  

### A small brief on how it works  
- The MCU reads data from sensors (line sensors, color sensor, proximity sensor, etc.) using its input pins (digital or analog).  
- It executes programmed logic (C/C++ or Arduino code) to make decisions. 
- A microcontroller is programmed using an IDE (Integrated Development Environment), the most common IDE is **Arduino IDE**.
- Few sophisticated IDEs are **platform.io** with VS code, **ESP-IDF** and **STM32CUBEIDE** (tailor made for esp and stm respectively). 
- Based on logic, it outputs PWM, direction signals, or digital commands to drivers/servos.  
- It also handles communication (Bluetooth, UART, I2C, SPI) between modules.
- Arduino is an 8-bit MCU whereas ESP and STM are 32-bit (esp32 stm32).  

### Common options  

- **Arduino UNO / Nano (ATmega328P)** – beginner-friendly, cheap, widely used.  
- **ESP32** – dual-core, built-in WiFi/Bluetooth, higher ADC resolution, useful for advanced robots.  
- **STM32 (e.g., STM32F4 series)** – powerful ARM Cortex MCUs, used in more professional robots.  


### Blogs or tutorials to help with  

#### Blogs
- [Arduino Getting Started Guide](https://docs.arduino.cc/learn/starting-guide/getting-started-arduino/)  
- [ESP32 Tutorials on RandomNerdTutorials](https://randomnerdtutorials.com/getting-started-with-esp32/)  
- [STM32 blog](https://evelta.com/blog/stm32-programming-a-comprehensive-beginners-guide/?srsltid=AfmBOoq6x6sDozfvQbin9zEuoSJ7CWzmdqedhFT0f7GBgPcxW2sEdn_Y)  



#### Videos
ARDUINO 101:
[Arduino crash course by Mark Rober](https://youtu.be/yi29dbPnu28?si=bGkHyEc_jc2YfsdQ)
[Arduino explained](https://youtu.be/nL34zDTPkcs?si=jBYP2hmtYfZDIv27)
[Arduino in 100 seconds](https://youtu.be/1ENiVwk8idM?si=BJkQPt4Mx9jdzNz_)
(what is a microcontroller and why does it exist - HIGHLY RECOMMENDED FOR BEGINNERS)


[How to power your arduino](https://youtu.be/I7MrL5Q7zvY?si=SyaA-xw7NjPpD_wB)


ESP32 101:
[Arduino to ESP](https://youtu.be/RiYnucfy_rs?si=UNdRZxPcuVwlPSxW)
[Esp driver fix](https://youtu.be/X3uwQo3NEhw?si=Rqd4jUiGa11Hf_W8)
[ESP32 platformIO - VS code](https://youtu.be/tc3Qnf79Ny8?si=8OPzIRCIH8HKKWIb)


STM32 101:
[STM32](https://youtu.be/2OwUnupABec?si=vmNiSuqTRprDeM8l)

