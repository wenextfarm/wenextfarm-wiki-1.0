---
title: Control Relays
description: 
published: true
date: 2026-07-08T10:00:12.808Z
tags: 
editor: markdown
dateCreated: 2026-07-08T09:58:30.747Z
---
You can use a **relay** in combination with your FarmBot's **Arduino** or [Farmduino](Farmduino) electronics board to turn on or off high-powered peripherals or devices that plug into a standard wall outlet. Example devices you could control with a relay include fans, window opening mechanisms, grow lights, heating elements, even :coffee: makers!

We recommend purchasing a 110V relay such as the [Controllable Four Outlet Power Relay](https://www.adafruit.com/product/2935) (pictured below) and then:
1. Plugging the relay into a power source such as an extension cord,
2. Connecting the peripheral to the relay's output, and
3. Wiring the relay up to spare digital I/O pins on your electronics board.

![110v relay switch](_images/110v_relay_switch.jpg =700px)

You can then control the peripheral from sequences with the [control peripheral command](https://software.farm.bot/docs/peripherals-and-sensors-sequence-commands) or by adding it to the [peripherals widget](https://software.farm.bot/docs/controls#peripherals).

> **⚠️ Consider the rain:** Please note that while FarmBot is designed to withstand the elements, the relay and peripheral you choose may not be. Because of this, you might consider only using relays and additional peripherals in an indoor environment.
