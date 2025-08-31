# Line Following Division

## Introduction
Just like the 👀**eyes** help humans see and follow a path, this division enables the robot to detect and track the line on the arena.  

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
  An IR module basically consists of an emitter and a receiver, IR radiation is emitted and if it is reflected by an object, it is recieved and indicates the presence of an obstacle / object.In this case 

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
- [TCRT5000 5 channel ir array](https://robu.in/product/tcrt5000l-5-channel-tracking-sensor-tracking-module-infrared-sensor/)
- [DIY Line Follower with TCRT5000 (Instructables)](https://www.instructables.com/Make-a-FAST-Line-Follower-Robot-Using-PID/)  
