---
title: Use the FarmBot Genesis Rotary Tool
description: **In this guide:** See how to use the FarmBot Genesis rotary tool
published: true
date: 2026-07-13T05:41:14.696Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T07:15:10.612Z
---

FarmBot Genesis v1.6+ kits include a **[rotary tool](https://genesis.farm.bot/docs/rotary-tool)** featuring a 24 volt DC motor, interchangeable implements, and an adjustable motor angle allowing FarmBot to perform light duty weed whacking, soil surface milling, and drilling operations.

<iframe class="embedly-embed" src="//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2Ff_GqlMAMWPk%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3Df_GqlMAMWPk&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2Ff_GqlMAMWPk%2Fhqdefault.jpg&key=02466f963b9b4bb8845a05b53d3235d7&type=text%2Fhtml&schema=youtube" width="854" height="480" scrolling="no" frameborder="0" allowfullscreen></iframe>

![rotary tool](/web/docs/how-to-guides/_images/rotary_tool.png =700x)

# Controlling the rotary tool

The rotary tool's motor can be activated using a peripheral pin:

- Pin 2 is used for forward operation
- Pin 3 is used for reverse operation

These pins can be used in either `Analog` or `Digital` modes, where a digital ON will result in full-speed operation while an analog value between 0 and 255 will result in a proportional speed from 0 to 100%.

You can set Pin 2 or Pin 3's mode and value in several ways:

## Manual control

To manually control the rotary tool, open up the [peripherals tab](../../app/controls/peripherals.md) of the controls popup. From there, you can configure Pins 2 and 3 to be in `Analog` or `Digital` mode and manually control them using the toggle switches or sliders.

> **ℹ️ Note:** 
> 
> Activating both Pin 2 and Pin 3 at the same time will result in the rotary tool not moving. While this will not cause any damage, it is not recommended.
{.is-info}


![rotary tool manual control](/web/docs/how-to-guides/_images/rotary_tool_manual_control.png =700x)

## Sequence commands

You can also control the rotary tool programatically using the following sequence commands:

- <span class="fb-step fb-write-pin">CONTROL PERIPHERAL</span>
- <span class="fb-step fb-write-pin">TOGGLE PERIPHERAL</span> (only toggles between Digital ON and OFF)
- <span class="fb-step fb-if-statement">LUA</span> using custom code. See our [developer documentation](http://lua.farm.bot/) for additional details.

![rotary tool control peripheral](/web/docs/how-to-guides/_images/rotary_tool_control_peripheral.png =700x)
![rotary tool toggle peripheral](/web/docs/how-to-guides/_images/rotary_tool_toggle_peripheral.png =700x)
![rotary tool lua](/web/docs/how-to-guides/_images/rotary_tool_lua.png =700x)
