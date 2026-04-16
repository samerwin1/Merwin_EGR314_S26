---
title: Welcome
tags:
- tag1
- tag2
---
<center>
<font size= "6"> Seth Merwin Datasheet </font><br>
as part of<br>
<font size= "8"> Project E-Fish-&-Sea </font><br>
for<br>
<font size= "5"> Team 201 </font><br>

**Submission: March 7, 2026**
</center>

## Introduction

The purpose of this datasheet is to document the design process of the Distance-Sensing LiDAR Subsystem for the greater E-Fish-&-Sea project. This subsystem is one part in a large group of interconnected embedded systems working together to acheive the end-goal of the project.

### Project Summary

The goal of the E-Fish-&-Sea project is to create an aquatic drone prototype which can be used for general exploration/research purposes. The main focus is that the drone will be able to explore areas unreachable/uninhabitable by humans, take pictures, and collect data about the environment. The project is split up into four subteams:

* Subteam A: Wifi & Human Interface
* Subteam B: Movement & Propulsion
* Subteam C: Camera & Positioning Arm
* Subteam D: Research & Development

Each subteam has two to three team members. Each member is in charge of their own individual subsystem inside that subteam. To learn about the project as a whole and/or view the datasheet for each other individual's subsystem, visit the [Team Website](https://egr314-s-2026-201.github.io/).

### My Contribution

I am one member of Subteam D: Research and Development. This subteam is committed to providing sensing capabilities to the drone in order for the user to view and collect environmental data. My personal responsibility for this project is the design and creation of a subsystem which can measure the distance to whatever object is in the path of the drone. This data is then sent through a UART serial communication chain to the human interface for viewing by the user. To acheive this goal, my subsystem makes use of a serial single-point LiDAR sensor which is controlled and processed by an 8-bit microcontroller. This datasheet provides documentation for the entire design process of the subsystem from founding requirements to the finished product.

### Directory

* To view the requirements that built the foundation of the module, visit the ["Requirements" page](https://samerwin1.github.io/Merwin_EGR314_S26/01-Requirements/Requirements/).
* To understand the physical components of the module and how they are connected, visit the ["Block Diagram" page](https://samerwin1.github.io/Merwin_EGR314_S26/02-Block-Diagram/Block-Diagram/).
* To view the chosen major hardware components of the module, visit the ["Component Selection" page](https://samerwin1.github.io/Merwin_EGR314_S26/03-Component-Selection/Component-Selection/).
* To see a breakdown of specifications for the module's microcontroller and why it was chosen, visit the ["Microcontroller Selection" page](https://samerwin1.github.io/Merwin_EGR314_S26/04-Microcontroller-Selection/Microcontroller-Selection/).
* To understand how power is supplied and disributed throughout the module, visit the ["Power Budget" page](https://samerwin1.github.io/Merwin_EGR314_S26/05-Power-Budget/Power-Budget/).
* To view the list of materials used to build this subsystem, and details about each component, visit the ["BOM" page](https://samerwin1.github.io/Merwin_EGR314_S26/06-BOM/BOM/).
* To see a detailed schematic of the electrical connections/circuitry for the subsystem, and see the design of the physical circuit board, visit the ["Schematic and PCB" page](https://samerwin1.github.io/Merwin_EGR314_S26/07-Schematic%20and%20PCB/schematic/).
* To see the message types that this subsystem receives/sends out along the serial communication chain between subsystems, visit the ["API" page](https://samerwin1.github.io/Merwin_EGR314_S26/08-API/API/)
* For additional supporting information left out of the main pages of the datasheet, visit the ["Appendix" page](https://samerwin1.github.io/Merwin_EGR314_S26/Appendix/).