---
title: Farmduino
description: 
published: true
date: 2026-07-08T10:00:12.808Z
tags: 
editor: markdown
dateCreated: 2026-07-08T09:58:30.747Z
---
![](_images/farmduino.jpg =700x)
![](_images/farmduino_2.jpg =700x)
![](_images/farmduino_3.jpg =700x)
![](_images/farmduino_4.jpg =700x)
![](_images/farmduino_data_cable.jpg =700x)
![](_images/farmduino_production_2.jpeg =700x)
![](_images/farmduino_production_3.jpeg =700x)

> The Farmduino microcontroller features a board layout and connectors that are optimized for FarmBot. It receives G-code commands from the Raspberry Pi and then moves the motors, reads sensors, activate peripherals, and more. It features integrated Trinamic TMC2130 stepper drivers for ultra quiet movements and an STM32 coprocessor dedicated to monitoring the rotary encoders.

## 规格参数

| 属性 | 值 |
|------|-----|
| Microcontrollers | ATmega2560, STM32 |
| Stepper Drivers | Trinamic TMC2130 |
| Input Voltage | 24V |
| Fuse | 7.5 amp blade fuse |
| Power Receptacle | Black 3-pin receptacle (<a href="https://www.molex.com/molex/products/part-detail/pcb_headers/2002411113">Molex Part 2002411113</a> |
| Vacuum Peripheral Receptacle | Black 3-pin receptacle, Molex part <a href='https://www.molex.com/molex/products/part-detail/pcb_headers/2002411113'>2002411113</a> (prior to January 2023) or <a href='https://www.molex.com/molex/products/part-detail/pcb_headers/0705430037'>705430037</a> (January 2023 and later) |
| Water, Lighting, and Peripheral 4 and 5 Receptacles | Black 2-pin receptacle (<a href="https://www.molex.com/molex/products/part-detail/pcb_headers/1510481206">Molex Part 151048-1206</a>) (prior to July 2022), Black 2-pin receptacle (<a href="https://www.molex.com/molex/products/part-detail/pcb_headers/0705430036">Molex Part 70543-0036</a>) (July 2022 and later) |
| UTM Receptacle | Black 12-pin receptacle (<a href="https://www.molex.com/molex/products/part-detail/pcb_headers/0430451212">Molex Part 430451212</a>) |
| UTM shunts | 8 1x2 2.54mm shunts pre-installed on UTM pins A through H |
| Motor Receptacles | Black 4-pin receptacle (<a href="https://www.molex.com/molex/products/part-detail/pcb_headers/0705430038">Molex Part 705430038</a>) |
| Encoder Receptacles | Black 7-pin receptacle (<a href="https://www.molex.com/molex/products/part-detail/pcb_headers/0705430041">Molex Part 705430041</a>) |
| Rotary Tool Driver | <a href="https://www.ti.com/lit/ds/symlink/drv8876.pdf">Texas Instruments DRV8876</a> H-bridge motor driver with integrated current sense and regulation |
| DC Current per I/O Pin | 40 mA |
| DC Current for 3.3V Pin | 50 mA |
| PCB color | Black |
| RoHS Compliant | Yes |
| CE Certification | Yes (<a href="https://drive.google.com/file/d/16wXEbiY1xF6eznnHQbq_53pAWcq5jr2P/view?usp=sharing">Certificate of Conformity</a>) |

**价格:** $195.00
**数量:** standard: 1 | xl: 1
**CAD 模型:** [在线预览](https://cad.onshape.com/documents/6626b842adca229e69544ad1/w/89ac2637f82d915f22c2bcd0/e/9b5558bc8c564860812b0723?renderMode=0&uiState=6255da12582c8d091a1f6dad)

## 内部规格

- **internal-part-name:** Farmduino v1.6
- **rev:** A
- **vendor:** LDO
- **cost:** $89.00
- **notes:** "<span style='color: red; font-weight: bold;'>QA check to ensure UTM Shunts are pre-installed</span>, Due to connector shortage, switched to smaller more readily available 2-pin connectors for peripherals (all but vacuum) via an adapter board for production 2 kits. Continued using 2-pin connectors and a new 3-pin connector for the vacuum pump for production 3."
