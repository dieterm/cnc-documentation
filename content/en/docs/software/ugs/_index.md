---
title: Universal G-code Sender
description: >
  TODO usefull description for Universal G-code Sender
date: 2024-11-25
weight: 3
---

{{% pageinfo %}}
This is a placeholder page that shows you how to use this template site.
{{% /pageinfo %}}

[Setup a Touch Probe With a Arduino CNC Shield and Grbl and UGS Platform](https://www.instructables.com/Setup-a-Touch-Probe-With-a-Arduino-Cbc-Shield-and-/)

[Making TOOLPATHS and exporting G-CODES | Fusion 360](https://willysgaragenorway.no/2018/01/12/making-toolpaths-and-exporting-g-codes-fusion-360/)

[Using G-CODE files and setting ZERO in UGS](https://willysgaragenorway.no/2018/01/23/using-g-code-files-and-setting-zero-in-ugs/)

[Tool Offsets with Tool Setter Probe in UGS Macro](https://www.youtube.com/watch?v=-2jFvlvu0co)

```gcode
G92.1; G90; G53 G0 Z0; G59; G0 X0 Y0; G0 Z0; G91; G38.2 Z-90 F300; G0 Z2; G38.2 Z-10 F30; G4 P.25; G38.4 Z10 F20; G4 P.25; G38.2 Z-10 F10; G4 P.25; G38.4 Z10 F5; G4 P.25;  G92 Z0;  G0 Z5 F3000; G90; G53 G0 Z0 F3000; G54;
```
