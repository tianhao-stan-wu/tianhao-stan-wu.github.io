---
layout: page
title: Ultrasonic Ranger/Fall Detector
description: Embedded system class project
img: assets/img/project5/rangefinder.png
importance: 2
category: class project
---

**Fall Detector** (Senior capstone project)

A comprehensive project [[report]](/assets/pdf/project5/fall_detect_report.pdf)

We developed The SafeStep Fall Detection Device, a tool designed to help detect falls. Of course, it's just a proof of concept :) . Components include:
1. LCD Display
2. Potentiometers for adjusting brightness and contrast
3. System status LED
4. Accelerometer and Gyroscope
5. Vibrator
6. Buzzer
7. 2x Buttons
8. Atmega328P Microcontroller

Below is a short demo for the detector. (**note**: increase volume to hear vibration and buzzing)


<iframe width="672" height="378" src="https://youtube.com/embed/JjxDg78UQEY?si=8Xqr4w98QEL1_C0Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<br>
<br>

**Ultrasonic Ranger**

Per instructors' requirements, I'm not allowed to share the source code publicly, which might result in unintended plagiarism. For writeup of the project, please go to [class website](https://bytes.usc.edu/ee109/project-spring23/) here.

Brief description:

1. measure distance up to 4 m
2. press the button to acquire a new measurement
3. rotate the rotary encoder to adjust local and remote thresholds
4. sevor motor acts as a second display for the measurement
5. green light if measurement > local, red light if measurement < local, blue light if no measurement or out of range
6. buzzer sounds if measurement < remote


Below is a short demo for the rangefinder.

<iframe width="672" height="378" src="https://www.youtube.com/embed/x4xZiXHliTI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>