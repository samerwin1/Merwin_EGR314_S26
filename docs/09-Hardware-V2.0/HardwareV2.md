---
title: Hardware V2.0
---

## Overview

Looking at the subystem's final state, there are several hardware design choices that could be improved. Some possible improvements are discussed below.

**Size Optimization**

The size of the physical printed circuit board could be reduced in order to save space on the drone. In a new hardware version, more time would be spent optimizing the PCB with smaller components and less space between them. Rather than soldering by hand, components would be soldered by machines in the factory. This would also improve accuracy, efficiency, and professionalism.

**Swap Out Prototyping Hardware**

Now that the subsystem has been tested and verified, the next version would remove the extra I/O sockets and the headers for the SNAP Debugger as they are no longer needed. The standard female sockets connecting the LiDAR sensor to the board would be replaced, either by soldering the sensor wires straight to the board or by installing a secure clipping connecter. These improvements would get rid of unnecessary clutter and ensure that the sensor does not become detached from the board.

**Motor/Shaft to Move Sensor**

This is something that was originally considered as a stretch requirement for the subsystem, but did not come to fruition due to project scope and budget limitations. In a future design, the LiDAR sensor would be mounted on a rotatable vertical shift driven by a motor. This motor could be controlled by the user to point the distance sensor in different directions relative to the drone's orientation. This would allow for improved scouting and environmental scanning capabilities.

**Interrupt-Enabled Pins**

During the design of the subsystem block diagram, schematic, and PCB the general input/ouput pins for the LEDs and debugging pushbutton were chosen rather arbitrarily. After the PCB was manufactured and the pushbutton was soldered, it was realized that the specific microntroller pin connected to the button did not support interrupt-on-change capability. This made it harder to reliably use the button for debugging and required more coding to get it to work properly. While this was not such a big problem, it is still something that would be changed in a new version.
