Selecting the right batteries for embedded projects and robotics requires careful consideration of the load, component datasheets, current requirements, voltage endurance, and the battery’s C rating. The following report outlines the structured approach, key decision factors, and reference materials for effective battery selection in such applications.

https://www.n-denkei.com/india/topics/product_info/3264/
https://husarion.com/blog/batteries-for-mobile-robots/
https://manlybattery.com/choosing-the-right-robot-battery-a-ultimate-guide/

## Determining the Load Requirements
- Before choosing a battery, it is essential to calculate the total power consumption of the system under various operating scenarios.
- Summing up the current required by all components: motors, sensors, processors, communication modules, and other accessories
- Measuring both peak and average expected current draws, as robotics and embedded systems often have dynamic loads (e.g., motors may require high current during    startup or rapid movement)
- Considering operational runtime goals to estimate required battery capacity (in ampere-hours, Ah).

## Reading Component Datasheets
- When analyzing datasheets for components (motors, ICs, regulators).
- Identify maximum rated current and voltage specifications for safe and reliable operation.
- For switching devices (MOSFETs, relays, drivers), ensure their maximum ratings surpass the highest expected load plus a safety margin (typically 20–30% extra is   recommended)
- Double-check voltage tolerances, as exceeding these can cause permanent damage, while operating well below rated voltage may cause malfunction or instability.

## Voltage Withstand Capability
- Assess the following for voltage selection:
- Match the battery’s nominal voltage to the system requirements (e.g., 7.4V for 2S Li-Ion/LiPo packs, 12V for lead acid or higher-voltage robot platforms)
- Verify that all downstream components tolerate the maximum fully charged voltage; for example, Li-Ion batteries may charge up to 4.2V per cell (8.4V for 2S),
  while most devices expect nominal cell voltage (3.7V per cell).

## Understanding Battery C Rating and Choosing Appropriately
- What is C Rating?
- The C rating quantifies how quickly a battery can be discharged relative to its capacity. A battery with a capacity of 1000mAh (1Ah) and a C rating of 10 (10C)
  can theoretically supply up to 10A safely.
- It’s vital for applications with high current demands or short bursts of peak power (motors, actuators)
- https://www.invertekenergy.com/what-is-c-rating-in-battery-a-guide-to-c10-and-beyond/
- https://www.pretapower.com/battery-c-ratings-guide-unlocking-the-science-behind-performance-and-efficiency/
- Calculate required discharge rate: For example, if total peak load is 8A and battery is 2000mAh (2Ah), minimum required C rating = 8A/2Ah = 4C.
- Select a battery with a higher C rating than calculated to allow a safety buffer and minimize stress on the battery, which extends its life.
- For control boards or sensors with low and steady power draw, low C rating batteries (C5–C20) suffice; for drive motors or active robotic arms, higher C rating
  (C10–C50 or more) is needed.
- C rating impacts both performance (high C for fast, responsive robotics) and longevity (lower C for steady, longer runtime).
- https://youtu.be/4qIYyaRKGVE?si=ksubmSPCQ4fLZJ5z
- https://youtu.be/cxkVxi9P0EA?si=nUjOnZRLjMaRgzDZ

  
## Useful Resources
- Learning about how you have to think intuitively.
- https://www.youtube.com/watch?v=Iye4uVLmj8o
- https://www.youtube.com/watch?v=IT19dg73nKU
  
- LIPO :
- https://youtu.be/Lk7wzVYmXSA?si=lTLMoxQMhIT-aQDK
- https://youtu.be/arOXg7y6r8k?si=Pb2ru-8dAzZspAyl
- (talks about lipo types and how to select one, LIPO is really great but it is very important on how you design)

- Clear understanding of the basics are crucial for further debugging/development.
- https://youtu.be/IT19dg73nKU?si=3DD5FhmGOrG8jrBz
- different batteries
- https://youtu.be/5C3R7VWO1Bo?si=qcLUiYwL0JQezYpB
- https://youtu.be/jgUVTZJyzoo?si=ymesC_FbXvpbry2j

- https://www.youtube.com/watch?v=EnokkBZmPQw  How to NOT Blow Up Your Robot - Motors, Batteries, ESCs and More Explained!

