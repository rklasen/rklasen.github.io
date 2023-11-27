---
title: "Homemade ESP 01 Dimmer"
date: 2022-10-28T13:48:10+02:00
draft: false
summary: "Why buy something that works when you can build it yourself for twice the price?"
tags: [Tasmota, ESP8266, Electronics]
toc:
  enable: true
  auto: true
images: [new-PXL_20220325_072404598.jpg]
featuredImagePreview: "new-PXL_20220325_072404598.jpg"
linkToMarkdown: true
---

Why buy something that works when you can build it yourself fot twice the price?

## First manual attempt

![Manual front](new-PXL_20220224_132238000.jpg)

![Manual back](new-PXL_20220224_132244306.jpg)

![3D Printed Case](new-PXL_20220224_132140139.jpg)

## A bit more professionalism, please!

![Scematic](schematic.png)

![PCB Front](pcb-0-front.png)

![PCB Back](pcb-0-back.png)

![Produced PCBs](new-PXL_20221028_115233629.jpg)

![Assembled](new-PXL_20220325_072404598.jpg)

## Second Version, not produced yet.

![PCB Front](pcb-front.png)

![PCB Back](pcb-back.png)

## Tasmota Template

```
{"NAME":"ESP01-DimmerRK","GPIO":[1,1,416,1,1,1,1,1,1,1,1,1,1,1],"FLAG":0,"BASE":18}
```

# References