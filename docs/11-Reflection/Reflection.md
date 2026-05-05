---
title: Reflection
---

## Review of Module's Sucess

The subsystem was an overall success. The module requirements table is copied below with an additional box showing whether the requirement was met or not in the final version of the module.

| **Requirement Description** | **Measure of<br> Threshold** | **Target<br>Measure** |**Stretch<br>Requirement<br>(Y-N)**|**Requirement<br>Met(Y-N)**|
|-----------------------------| ----------------- | ----------------- | :-----: | :-----: |
| 1. Surface mounted, 3.3V switching power regulator | 3.2 Volts | 3.3 Volts | No | Yes(3.3V) |
| 2. Surface mounted microcontroller | 1 PIC or ESP | 8-bit PIC | No | Yes(8-bit PIC) |
| 3. Serial sensor | Capable of quick and accurate distance sensing | LiDAR ToF sensor | No| Yes(LiDAR) |
| 4. Able to determine distance from device to object in its path | 10 ft range | 20 ft range | No | Yes(26ft) |
| 5. Wired communication | Able to send distance data to another subsystem | Send distance data to subsystem A2 through serial communication (UART) | No | Yes(UART) |
| 6. Sufficient refresh rate | Read/send out distance values at 1Hz | Read/send out distance values >10Hz | No | Yes<br>(>10Hz possible) |
| 7. Multi-directional | Able to read distance in more than 1 direction relative to device orientation | 360-degree distance sensing on horizontal axis | Yes | No |

As seen from the table the only requirement that was not met is the Multi-directional capability, which was a stretch requirement(goes beyond realistic limits, not necessary for success). This was a good idea that would have been nice to acheive, but it was unrealistic due to the scope, time, and budget limitations of the project. All of the necessary requirements for the subsystem met or exceeded the target measures for success. That being said, due to constraints on the amount of messages the team could send through the 10-person UART chain, we ended up only sending the distance value to the human interface once every two seconds. Therefore this requirement was technically not met when the subsystem was used in the prototype although it had the capability to exceed it.

## Microcontroller/Module Startup Tips

* **Check your hardware!** Personally there have been several times throughout this course and others where I've spent way too much time trying to understand why a circuit/code wasn't working, just to realize that I had a bad breadboard/solder connection. If it seems like you're doing everything right and something just refuses to work, save yourself time and stress by double checking all of your hardware connections.
* **Read datasheets carefully.** Make sure that you can find a reputable/correct datasheet for any part you're not totally familiar with and ensure you understand the information you need from them. Mistakes can be made easily by not being able to find the info you need or misreading/misunderstanding it.
* **Find support online.** Before settling on a major idea for your subsystem with a specific microcontroller/components, make sure you can find an example of somebody successfully implementing that combination. Obviously the point of the course is to create something original and figure it out yourself, but it's nice to have a reference or backup plan just in case you can't figure out how to do it.

## Top 10 Lessons Learned

1. Due to the amount of different component types I had on the top and bottom of my board, I learned a lot of techniques for soldering surface mount components. I now feel much more confident in my soldering abilities.
2. I learned a lot about I2C communication. While struggling to get my microcontroller to communicate correctly with my distance sensor, I dove deep into how the protocol works and gained a much fuller understanding. I now feel ready to work with I2C for future projects.
3. Software interrupts were something I had heard about but never touched before this course. I thought that they were going to be very technical/confusing, but this course helped me learn how to use them rather easily and see just how valuable they are.
4. I learned that just because something works once or even a couple of times, that doesn't mean it's guaranteed to work in the future. The first time the team connected our boards together the communication worked almost flawlessly. Then the second time, we had some bugs but fixed them and thought it was all good. Then on the day of the showcase things randomly were not working. We should have spent more time testing to make sure we caught everything and could get consistent function.
5. This class reinforced my opinion that a bigger team doesn't necessarily make a project easier. While it is useful to have many group members to help eachother and come up with ideas, it also gets complicated when trying to ensure compatibility between everyone and stay on the same page.
6. Between this course and EGR 304, I learned the importance of detailed/organized documentation of a project every step of the way. There were many times I needed to reference something I had done weeks/months beforehand and could not remember exactly what I did. Having the website to reference with everything in one place was super beneficial.
7. While my subsystem used the Microchip microcontroller and C programming, this course helped me start learning Python. The language is one that I never got experience with but have been interested in learning. The labs in this class forced me to start using it and get a basic understanding of the syntax.
8. I learned the importance of continuity testing and how it works. It was never taught to me and I did not understand it until this semester. I asked someone to teach me, now I understand how simple it is and how it is used to verify circuits before powering them.
9. I learned how to write a program that could intercept coded messages and filter/decipher them into something meaningful. I have never had to do something like that before and I found it to be interesting, challenging, and rewarding once I figured it out.
10. Finally, I rediscovered the importance of having teammates of different backgrounds/expertise. Usually when somebody needed help with something specific in this group, somebody else was highly skilled/knowledgeable on that topic and could help find the solution while teaching them things in the process. Additionally, we were often able to look at problems from different perspectives and supplement eachother to come up with the perfect solution.


## Recommendations for Future Students

1. Look at some explanations/examples of software interrupts before the assignments/lectures in class. It helps to have an understanding of how they work before jumping right into it with the lab, and they are a vital tool in programming.
2. Get at least a light understanding of advanced serial communication modes (SPI and I2C) before getting too far into this course. It is more complicated than UART and will take some time to get it working smoothly/correctly.
3. Try to select and order your microchip/components well before the assignment due date with through-hole versions so you can begin building your system on a breadboard and debugging. This way you can work out all the kinks before your PCB arrives and you don't have to stress about your subsystem not working in the final weeks.
4. Similar to #3, try to get a headstart on designing your PCB, finish it well before the due date, and review it with the professor/student-aids/classmates. It is imperative that you find errors before the designs are sent out to be printed so that you don't fry components and/or end up having to physically alter your PCB with very little time left in the semester.
5. Coordinate with your teammates to get your individual subsytems finished and connect them together for testing. You will want multiple sessions for testing to ensure compatibility and consistent results before the in-class checkoff/Innovation Showcase.