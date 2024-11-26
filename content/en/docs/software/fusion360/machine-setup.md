---
title: Machine setup
description: TODO usefull description for machine setup
date: 2024-11-25
weight: 2
---

{{% pageinfo %}}
This is a placeholder page that shows you how to use this template site.
{{% /pageinfo %}}

[Basic CNC with Fusion360, Candle, GRBL, Genmitsu 4030 and the mystery of G54! - wooden plant labels](https://www.youtube.com/watch?v=Yjken5DIyY4&list=PLM9-roy6qPn-A4EyFudR6iccRoVeNgSH6&index=4)

```
G-code I used to set G54 on my machine

G10 G54 P1 L2 X-383 Y-171 Z-44

G10 = set offset command
G54 = specific work offset location
P1 = parameter address (P1 is associated with G54 I think!)
L2 = informs G10 we are setting work offsets (as opposed to tool offsets)
```
