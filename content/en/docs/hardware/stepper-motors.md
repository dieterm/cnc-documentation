---
title: Stepper Motors
description: >
  TODO usefull description for stepper motors
date: 2024-11-25
weight: 5
---

Nema 23
Model: SMNM23S18KG13
Power: 4A
Torque: 12.85kg/cm

paar 1: zwart (A+) groen (A-)
paar 2: rood (B+) blauw (B-)

1,8°/step
360°/1,8 = 200 steps per revolution

ballscrew SFU1605
-> pitch = 5mm/rotation

stepperdriver TB6600
-> 16 microsteps/step

## X-as en Y-as

steps per mm = (200steps x 16 microsteps) / 5mm = 640 microsteps / mm

## Z-as

pitch = 2mm/rotation

steps per mm = (200 x 16) / 2mm = 1600 microsteps / mm
