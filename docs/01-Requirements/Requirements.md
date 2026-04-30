---
title: Subsystem Requirements
---

## Module Requirements
This page documents the requirements that the distance-sensing subsystem must fulfill in order to achieve its goals relating to the greater project. Each entry in the table below describes one requirement, the minimum measurement threshold that must be met, the target measurement for success, and whether it is a stretch requirement(goes beyond realistic limits; not necessary for success) or not.

| **Requirement Description** | **Measure of<br> Threshold** | **Target<br>Measure** |**Stretch<br>Requirement<br>(Y-N)**|
|-----------------------------| ----------------- | ----------------- | :-----: |
| 1. Surface mounted, 3.3V switching power regulator | 3.2 Volts | 3.3 Volts | No |
| 2. Surface mounted microcontroller | 1 PIC or ESP | 8-bit PIC | No |
| 3. Serial sensor | Capable of quick and accurate distance sensing | LiDAR ToF sensor | No|
| 4. Able to determine distance from device to object in its path | 10 ft range | 20 ft range | No |
| 5. Wired communication | Able to send distance data to another subsystem | Send distance data to subsystem A2 through serial communication (UART) | No |
| 6. Sufficient refresh rate | Read/send out distance values at 1Hz | Read/send out distance values >10Hz | No |
| 7. Multi-directional | Able to read distance in more than 1 direction relative to device orientation | 360-degree distance sensing on horizontal axis | Yes |
