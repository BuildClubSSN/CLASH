# Motor Control Division – Motor Drivers

## Introduction
Motors are the 🦵**legs** of the robot, but they cannot be powered directly by a microcontroller. 
 
The motor control division ensures smooth movement of the robot by providing the right amount of power and directional control to the motors.  
A motor driver is like the **nerves** and acts as the bridge between the **low-power control signals** from the microcontroller and the **high-power requirements** of the motors.  

---

## Why a motor driver is required
- A microcontroller can only provide low-power signals like PWM [Pulse Width Modulation](https://learn.sparkfun.com/tutorials/pulse-width-modulation/all) and direction control.  
- Motors need higher current and voltage than what the microcontroller pins can supply.  
- A motor driver amplifies these low-power signals using an external power supply and delivers sufficient current to the motors.
- motor drivers are powered using external power supply and not like other sensors which can be powered from microcontroller itself.  
- Motor drivers are usually based on the [H-bridge principle](https://www.build-electronic-circuits.com/h-bridge/), enabling both speed control (via PWM) and direction control.  
- **MOSFET-based drivers** are preferred over BJT-based drivers due to higher efficiency and better high-frequency performance.  

---

## How it works
- The microcontroller outputs PWM and direction signals.  
- The motor driver, using its **H-bridge circuit**, translates these into high-current signals.  
- By controlling the polarity of voltage supplied to the motor, the driver can rotate the motor **forward or backward**.  
- By adjusting the **duty cycle of PWM**, the driver controls motor speed.  

---

## Common options
- **L298N** – Old, BJT-based, less efficient, produces more heat but reliable.  
- **TB6612FNG** – Modern, MOSFET-based, efficient.  
- **DRV8833 / DRV8835** – Compact, efficient MOSFET-based drivers, ideal for battery-powered robots.  

---

## Selection guidelines
1. Select the motor first (e.g., BO motor or N20 motor).  
2. Define requirements: speed (RPM), torque, and operating voltage.  
3. Check **stall current** (maximum draw at startup or heavy load).  
4. Choose a motor driver with:  
   - Voltage rating matching the motor’s operating voltage.  
   - Continuous current rating higher than the motor’s running current.  
   - Peak current rating higher than the motor’s stall current.  
5. Decide how many motors to control; some drivers can drive **two motors simultaneously**.  

---

## Useful resources

- [Motor Driver Basics – Last Minute Engineers](https://lastminuteengineers.com/l298n-dc-stepper-driver-arduino-tutorial/)  
- [All you need to know about motors](https://www.youtube.com/watch?v=CjEYVcPu2vM)
  


