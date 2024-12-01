---
title: G-code Basics
description: More about G-code Basics
date: 2024-11-25
weight: 5
---

## G-code commands

### G10 G53 - G54, G55, .. G28 G30

[Understanding G-code Coordinate Systems](https://www.youtube.com/watch?v=fGtbkVJBXyE)

```gcode
Machine Coordinates (G53)

Work Coordinates (G54 -> G59)

Predefined positions (G28, G30)

$H                      (homing)
G91 X30 Y-120 Z-30      (Jogging, relative from active machine coordinates system)
G10 L20 P0 X0 Y0 Z0     (stel de huidige work coordinates in op 0,0,0. P0 betekend huidige working coordinates, en G54 is de default)
$#                      (toon een lijst met de huidige coordinate systems)
$G                      (geef status info, met onder andere het actieve coordinate system, bv. G54)
```

## G0, G1, G20, G21, G28

[TOP FIVE ** MUST KNOW ** G Codes You Will Use For & How To Use Them on your cnc, Router Laser, gcode](https://www.youtube.com/watch?v=e8BoMeNGfas)

```gcode
G0 (ga zo snel mogelijk naar een bepaalde positie)
G0 X0 Y0 Z0

G1 (ga naar een bepaalde positie, maar houd rekening met de opgegeven feedrates)
G1 X10 Y0 F500

G21 metric mode (millimeters)
G20 imperial mode (inches)

G90 absolute jogging
G90 X30 Y-120 Z-30

G91 relative jogging, from active machine coordinates system
G91 X30 Y-120 Z-30
```

## M-commands

[Understand G code for beginners Part 1](https://www.youtube.com/watch?v=bpNNaTUi_7c)

```gcode
M0          (Pause the machine, and resume again)
M2          (End the current program)
M3 S12000   (start spindle clockwise with 12000 RPM)
M4 S12000   (start spindle counter-clockwise with 12000 rpm)
M5          (stop spindle)
M8          (start watercooling or activate relay)
M9          (stop watercooling or deactivate relay)
M30         (stop program and rewind to first line)
```
