---
title: Farmduino
description: 
published: true
date: 2026-07-08T10:00:12.808Z
tags: 
editor: markdown
dateCreated: 2026-07-08T09:58:30.747Z
---
# Open-source

> **ℹ️ Connectors may vary:** Due to supply chain shortages of certain connectors, your Farmduino may have one of two connector types for the vacuum pump peripheral and all of the other peripherals. Please inspect the images above to note the differences and ensure you purchase cables with the correct connector type when ordering spare or upgrade parts.


|Resource|Link|
|--------|----|
|Schematics, board layout, and hardware source files|[Google Drive Folder](https://drive.google.com/drive/folders/1yilyUpWPxHwNqFovOlq9ZL7B2jPNqCCX?usp=sharing)
|Arduino MCU firmware source code|[GitHub](https://github.com/FarmBot/farmbot-arduino-firmware)
|STM32 firmware for tracking encoder signals|[GitHub](https://github.com/MotorDynamicsLab/encoder-tracker/releases/tag/v1.0.2)
|Pinout references|[Link](../../extras/reference/pinout-references.md)

**Component tests**{:.internal}

|Test         |Description  |Target       |Tolerance    |
|-------------|-------------|-------------|-------------|
|Pins         |Inspect the pins for damage.|No pins should be bent|N/A
|Fuse         |Ensure the blade fuse is inserted and of the correct amperage.|7.5 Amps|N/A
|USB power out|Read the voltage coming from the `POWER OUT` USB connector.|5.25V|+/- 0.1V
|UTM shunts   |Inspect for the presence of the UTM pin shunts.|Present on Pins `A`-`H`|N/A
|Color        |Inspect the color of the PCB.|Matte black|N/A
|Functionality|Use the factory test firmware to test motor, encoder, and peripheral functions.|All functions work|N/A
|Encoder tracking|Move all motor axes with manual controls, by hand, and with forced stalls.|Encoder positions should be accurately tracked in all scenarios.|N/A
|Encoder tracking range|Using stock encoder scaling, move to +/- 10,000mm on the X and Y axes and +/- 2,000mm on the Z axis.|STM32 should accurately track encoder positions through the range of movement.|N/A
|STM32 reset  |Set `pin 49` low and then high.|Encoder tracking should reset.|N/A
|SPI comms    |Move motors to random positions and then modify Trinamic TMC2130 parameters (eg: motor current)|Parameters should update and encoder tracking should maintain position.|N/A
