---
title: Module Schematic
---

## Overview

This schematic below is designed to indicate the electrical connections/circuitry of the LiDAR subsystem. The "Power Supply/Voltage Regulators" section shows that power can be taken from the team bus connection or a wall supply via barrel jack, and it is sent through two different voltage regulators: one to provide 5V and one to provide 3.3V. The "Team Ribbon Cable Connectors" section highlights the connections to team subsystems in and out for UART communication and shared power. The "MPLAB Snap Programming/Debugging Tool" section shows the tool which will be used to upload code to the microcontroller after soldering it to the PCB. The "TF-Luna Single Point LiDAR Sensor" section shows the chosen LiDAR sensor and its connections to the microcontroller, as well as the data addresses which will be used for I2C communication. Finally, the "PIC18F47K42-E/PT Microcontroller" section displays the chosen microcontroller for the subsystem, which of its pins connect to power/peripherals, two external status LEDs, one pushbutton for debugging purposes, and multiple extra headers connected to unused pins in the event that additions must be made to the system.


![schematic](IndividualSubsystemSchematicEGR314V2.png){style width:"350" height:"300;"}



## Resouces

The schematic as a PDF download is available [*here*](EGR314-IndividualSubsystemDesign-SAM.pdf), and the Zip folder of the project [*here*](EGR314-IndividualSubsystemDesign-SAM.zip).