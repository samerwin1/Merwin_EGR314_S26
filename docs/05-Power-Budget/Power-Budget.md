---
title: Power Budget
tags:
- tag1
- tag2
---

## Overview

This power budget shows the major power-drawing components of the subsystem and how sufficient power will be supplied to them.

[Power Budget](314-IndividualSubsystemPowerBudget.png)

The subsystem will be powered with a 9V 3A power supply feeding into two switching voltage regulators. The first regulator supplies 5V to the TF Luna LiDAR Sensor which has a maximum current of 150 mA. The second regulator supplies 3.3V to the PIC18F47Q43-I/PT microcontroller which has a maximum current of 350 mA. All other peripherals will be powered through the microcontroller and draw a negligible amount of current. This power budget shows that the chosen power supply will have more than enough current to supply both major components including safety margins for overdraws.

## Resources

The power budget is available as a pdf [here](314-IndividualSubsystemPowerBudget.pdf) and as an excel worksheet [here](314-IndividualSubsystemPowerBudget.xlsx).