---
title: Subsystem Block Diagram
tags:
- tag1
- tag2
---

## Overview
This page provides a block diagram representing the hardware components in the Distance-Sensing subsystem, how they connect to each other, and how they are powered. The microcontroller and all components are powered by a regulated 3.3V switching DC. Jumpers have been put in place to allow switching the source power between one individual to the subsystem(for prototyping purposes) and one shared by the team(for the final design). All logic and control inside the subsystem will be handled by the Microchip PIC18F47K42 surface-mount microcontroller. This subsystem wil make use of a single-point LiDAR ToF sensor to capture and process distance data, interacting with the microcontroller through I2C serial communication. The subsystem will use ICSP programming through the Microchip Snap debugger/programmer in order to update the software throughout the prototyping phase. Interaction with other subsystems will be through UART serial communication via one upstream ribbon connector and one downstream ribbon connector. One generic LED and generic pushbutton have also been added for subsystem status/debugging purposes.


## Block Diagram 

<center>
![Block Diagram](314IndividualBlockDiagram2.drawio.png)
</center>

A PDF version of the block diagram is available [here](314IndividualBlockDiagram2.pdf), and the original drawio file [here](314IndividualBlockDiagram%20(1).drawio).
