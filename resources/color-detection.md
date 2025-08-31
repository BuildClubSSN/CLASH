# Line Following Division

## Introduction
Line following is the foundation of most autonomous ground robots.  
In this competition, the bot must follow a **25 mm wide black line on a white surface** to navigate between different zones.  
The accuracy of line detection directly affects the performance of all other subsystems — from motor control to box placement — making this one of the most critical divisions in the design.  

---

## Why this sensor is required
- Enables the bot to **stay on track** and complete both phases of the event.  
- Detects **special patterns** like intersections, broken lines, and stop zones.  
- Provides **navigation state feedback** to the motor control system for smoother motion.  

---

## How it works
- Line following sensors rely on **Infrared (IR) reflectance**:  
  - **Black regions** absorb IR → sensor reads *low*.  
  - **White regions** reflect IR → sensor reads *high*.  
- Multiple sensors arranged in an **array** let the bot measure the exact position of the line.  
- This information is fed into a **PID controller** or similar algorithm for smooth corrections.  

---

## Common options
- **IR Sensor Arrays**
  - Pololu QTR-xA (analog) / QTR-xRC (digital RC)  
  - DIY TCRT5000-based arrays (affordable, widely available)  
- **Standalone IR Sensors**
  - TCRT5000 modules for detecting start/stop zones or intersections.  

---

## Useful resources
- [Pololu QTR Sensors Overview](https://www.pololu.com/product/961)  
- [TCRT5000 5 channel Ir array](https://robu.in/product/tcrt5000l-5-channel-tracking-sensor-tracking-module-infrared-sensor/)
- [Instructables-line follower](https://www.instructables.com/Make-a-FAST-Line-Follower-Robot-Using-PID/)