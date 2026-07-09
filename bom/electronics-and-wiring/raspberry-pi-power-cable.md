---
title: Raspberry Pi Power Cable
description: 
published: true
date: 2026-07-08T10:00:12.808Z
tags: 
editor: markdown
dateCreated: 2026-07-08T09:58:30.747Z
---
**Component tests**{:.internal}

|Test         |Description  |Target       |Tolerance    |
|-------------|-------------|-------------|-------------|
|Cable        |Inspect the cable spec.|`Shielded 28AWG/1p + 24AWG/2c`<br><br>`1p` = 1 twisted pair (for data)<br>`2c` = 2 core (for power)|N/A
|Connectors   |Connect the cable to a Raspberry Pi and Farmduino inside a fully assembled electronics box.|The cable should connect to both circuit boards without interference from the box or other components.|N/A
|Length       |Measure the length using a measuring tape.|300mm|+/- 5mm
|Voltage drop |Use USB voltage monitors to check the voltage before and after the cable.|Less than 5% voltage drop|4.9V output minimum
|Color        |Inspect the color of the cable.|Black or White|N/A


> **ℹ️ Some v1.6 kits include different Raspberry Pi Power Cables:** Genesis and Genesis XL v1.6 kits shipped before July of 2022 included a black Raspberry Pi Power Cable with a microUSB connector to plug into the Raspberry Pi Model 3B+. v1.6 kits shipped during or after July of 2022 included a white or black Raspberry Pi Power Cable with a USB-C connector to plug into the Raspberry Pi Model 4B.
