---
title: Status LEDs
description: The meaning behind the blinking
published: true
date: 2026-07-26T02:23:05.040Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T06:57:48.732Z
---

# Raspberry Pi LEDs

The Raspberry Pi has LED lights that convey information about its status.

![RASPBERRY PI LIGHTS](/web/farmbot-os/intro/_images/raspberry_pi_lights.jpg =700x)

_Raspberry Pi 3B+, included with Genesis kits_

|Red (power)                   |Status                        |
|------------------------------|------------------------------|
|<span class="fa fa-circle led red"></span> (solid red)|Good to go! You are connected to a 5V power supply via the Farmduino.
|<span class="fa fa-sun-o led red"></span> (blinking red)|Low power - Try a more powerful power supply or a different cable.
|<span class="fa fa-circle-thin led red"></span>  (off)|No power / low power - Plug in to a 5V, 3A power supply.

## Green (activity) LED

|Green (activity)              |Status                        |
|------------------------------|------------------------------|
|<span class="fa fa-circle led green"></span> (solid green)|Busy working/booting
|<span class="fa fa-sun-o led green"></span> (blinking randomly)|Busy working/booting
|<span class="fa fa-sun-o led green"></span> (blinking consistently)|Network disconnected or emergency stopped - [Configure FarmBot](configurator.md), press <span class="fb-button fb-yellow">UNLOCK</span> in the Web App, or check that the network FarmBot is connected to is online.
|<span class="fa fa-circle-thin led green"></span> (off)|Ready and waiting for the next task

# Electronics box LEDs

In addition to the LEDs located on the Raspberry Pi, Genesis v1.4+ kits feature LEDs mounted on top of the electronics box, and Express v1.0+ kits feature LEDs on the Farmduino Express circuit board.

![Box LEDs on Genesis kit](/web/farmbot-os/intro/_images/Box_LEDs_on_Genesis_kit.png =700x)

_Box LEDs on Genesis kit_

![LEDs on Farmduino express board](/web/farmbot-os/intro/_images/leds_on_farmduino_express_board.jpg =700x)

_Farmduino Express LEDs on Express kits_

## LED 1 (sync)

This green LED indicates the **sync status** between FarmBot and the web app. It is connected to Raspberry Pi GPIO BCM pin 24.

|Green (sync)                  |Status                        |
|------------------------------|------------------------------|
|<span class="fa fa-circle led green"></span> (solid green)|Synced and ready
|<span class="fa fa-sun-o led green"></span> (blinking slowly)|Needs sync (Will not execute any unsynced events or sequences)
|<span class="fa fa-sun-o led green"></span> (blinking quickly)|Syncing
|<span class="fa fa-circle-thin led green"></span> (off)|Offline - Check the connection status LED


# Electronics box buttons

Some kits also include push buttons featuring integrated LED lights.

## E-Stop Button

The **E-Stop Button** (included with all Genesis v1.4+ and Express v1.0+ kits) has a red LED that indicates if FarmBot is <span class="fb-button fb-red">E-STOPPED</span> or not. It is connected to Raspberry Pi GPIO BCM pin 17.

|Red (E-stop)                  |Status                        |
|------------------------------|------------------------------|
|<span class="fa fa-circle led red"></span> (solid red)|Unlocked and ready
|<span class="fa fa-sun-o led red"></span> (blinking red)|FarmBot is missing firmware. This is normal during configuration. If you have completed configuration, selected your FarmBot model in the [Message Center](../../app/intro/message-center.md) and still see blinking, you may need to flash the [Arduino Firmware](../arduino-firmware.md).
|<span class="fa fa-circle-thin led red"></span> (off)|Locked - Check the Unlock Button LED status

## Unlock Button

The **Unlock Button** (included on the top of the electronics box with all Genesis v1.4+ and on the Farmduino Express circuit board with all Express v1.0+) has a yellow LED that indicates if FarmBot is <span class="fb-button fb-yellow">UNLOCKED</span> or not. It is connected to Raspberry Pi GPIO BCM pin 23.

|Yellow (unlock)               |Status                        |
|------------------------------|------------------------------|
|<span class="fa fa-sun-o led orange"></span> (blinking)|Locked - When safe to do so, press this button to unlock FarmBot.
|<span class="fa fa-circle-thin led orange"></span> (off)|Unlocked and ready

## Other buttons

Some kits include three additional buttons (Button 3, Button 4, and Button 5) whose actions can be customized via the [push button UI](../../app/controls/peripherals.md#push-buttons), however the LEDs for these buttons are not customizable.
