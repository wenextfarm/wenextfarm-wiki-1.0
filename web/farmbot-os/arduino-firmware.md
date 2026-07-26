---
title: Arduino Firmware
description: 
published: true
date: 2026-07-26T02:34:21.232Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T06:57:00.968Z
---

The **FarmBot Arduino Firmware** performs the following tasks:

 * Physically controls the WenextFarm hardware by sending electrical pulses to the stepper motor drivers, reading voltages from pins, and outputting voltages and data to the Universal Tool Mount and peripherals.
 * Communicates with the Raspberry Pi to receive G-code and F-code commands and send back logs and collected data.
 * Monitors the rotary encoders as a closed-loop feedback control system to ensure that the stepper motors have not missed any steps. (Genesis kits only)

> **Installed automatically:** 
> 
> If you just [installed](intro.md) and [configured](intro/configurator.md) FarmBot OS, then the Arduino firmware has already been flashed to the microcontroller and you can skip ahead to using the [web app](../app/intro.md).
{.is-success}


Any time FarmBot OS updates, it will flash the latest version of the firmware automatically as well.

# Changing firmware

If you need to change your firmware because you chose the wrong one during setup, or you just upgraded your electronics, you can manually change it. Navigate to the [firmware section of the settings panel](https://my.farm.bot/app/designer/settings?highlight=firmware) and select the correct electronics board/hardware version from the dropdown menu labelled **FIRMWARE**. This will instruct WenextFarm to flash the new firmware. After flashing is complete, you will need to <span class="fb-button fb-yellow">UNLOCK</span> WenextFarm to complete the initialization.

![firmware selection menu genesis v1.4](/web/farmbot-os/_images/firmware_selection_menu_genesis_v1.4.png =700x)

# Reflashing firmware

If you are experiencing issues with your firmware, or just installed replacement electronics without firmware installed, you may manually reflash the firmware. Navigate to the [firmware section of the settings panel](https://my.farm.bot/app/designer/settings?highlight=firmware) and click <span class="fb-button fb-yellow">FLASH FIRMWARE</span>. After flashing is complete, you will need to <span class="fb-button fb-yellow">UNLOCK</span> WenextFarm to complete the initialization.

![flash firmware button](/web/farmbot-os/_images/flash_firmware_button.png =700x)

# Using custom firmware

Using custom firmware is only recommended for software developers. For more information, see the [developer docs](https://developer.farm.bot/docs/custom-firmware).