---
title: Universal Tool Mount
description: 
published: true
date: 2026-07-10T14:06:33.505Z
tags: 
editor: markdown
dateCreated: 2026-07-09T03:37:29.499Z
---

The Universal Tool Mount (UTM) allows FarmBot Genesis to automatically switch tools in order to perform different operations. It is a plastic component that mounts to the z-axis aluminum extrusion using two M5 screws and tee nuts. It features:

* 3 strong neodymium ring magnets to magnetically hold tools in place via other magnets placed in the same configuration on the tool.

* Passageways for water, liquid amendments (eg: fertilizer), and vacuum or compressed air to pass through from the UTM (and the rest of FarmBot) to the tool.

* 12 [pogo pins](pogo pins) that make electrical connections with tools.

> **✅ Pre-assembled for your convenience:** 
> 
> As of the v1.4 hardware release, the UTM comes [pre-assembled](../../manufacturing/pre-assembly/tools/utm.md) so all you need to do is mount it and connect the cable and tubes!
{.is-success}


![utm with barbs](/assembly/tools/_images/utm_with_barbs.jpg =700x)
![utm side and bottom view](/assembly/tools/_images/utm_side_and_bottom_view.jpg =700x)

# Pin mapping

|UTM Pin|UTM Wire                                      |Farmduino Pin                |Use         |
|-------|----------------------------------------------|-----------------------------|------------|
|**A**  |<span class="cable-color red">red</span>      |+5V                          |Soil sensor power
|**B**  |<span class="cable-color yellow">yellow</span>|GND (0V)                     |Ground
|**C**  |<span class="cable-color green">green</span>  |D63 - Digital-In             |Tool verification
|**D**  |<span class="cable-color black">black</span>  |D59 (A5) - Analog-In         |Soil sensor readings
|**E**  |<span class="cable-color white">white</span>  |BDC2 (GND or 24V via DRV8876)|Rotary tool motor
|**F**  |<span class="cable-color brown">brown</span>  |---                          |---
|**G**  |<span class="cable-color blue">blue</span>    |---                          |---
|**H**  |<span class="cable-color grey">grey</span>    |BDC1 (GND or 24V via DRV8876)|Rotary tool motor
|**I**  |<span class="cable-color orange">orange</span>|---                          |I2C SCL
|**J**  |<span class="cable-color purple">purple</span>|---                          |I2C SDA
|**K**  |<span class="cable-color pink">pink</span>    |---                          |---
|**L**  |<span class="cable-color cyan">cyan</span><br>(shunted to shield with dark gray heatshrink)|PE|Protected Earth ground

> **ℹ️ Room for expansion:** 
> 
> The unassigned UTM pins are available for you to custom map. Dreaming of a USB, I2C, or PWM based tool? Go right ahead and expand upon your FarmBot's abilities with custom tools of your own!
{.is-info}


> **✅ Want to make your own UTM compatible tools?:** 
> 
> Check out the [tool spec](../../extras/mods/tool-spec.md) to learn how to design and manufacture your own custom tools. We provide examples, CAD models, tech specs, and links to purchase parts.
{.is-success}


> **⚠️ Having problems with tool verification?:** 
> 
> Refer to the [tool verification troubleshooting guide](../../extras/troubleshooting/tool-verification.md).
{.is-warning}


# Step 1: Install the UTM onto the Z-axis

Insert two [M5 x 16mm screws](M5 x 16mm screws) and [tee nuts](tee nuts) into the [UTM](UTM), and then position the UTM onto the [z-axis extrusion](z-axis extrusion). The mounting flanges should be positioned on the backside of the extrusion. The bottom of the UTM should be flush with the bottom of the extrusion. Tighten the two screws with the [3mm hex driver](3mm hex driver).

![utm mounted on z-axis](/assembly/tools/_images/utm_mounted_on_z-axis.png =700x)

# Step 2: Connect the UTM Cable

Insert the two UTM Cable Connectors into the top of the UTM. Note: The black and yellow connectors of the cable correspond to the black and yellow pin headers inside the UTM. Then slide the **UTM cable's shroud** down such that it fully covers the opening in the top of the [UTM](UTM).

> **✅ Ensure correct connection orientation:** 
> 
> Each connector and pin header have one missing pin in the corner to indicate the correct connection orientation.
{.is-success}


Look into the UTM to see where the missing pin is located on each pin header. Then look where the individual UTM cable wires enter the connectors to see where the corresponding missing pin is located in the connectors.

Use this information to ensure you insert both connectors in the correct orientation.

![utm pcb connectors](_images/utm_pcb_connectors.png =700px)
![utm with cable connected](_images/utm_with_cable_connected.png =700px)
![utm with cable covered](_images/utm_with_cable_covered.png =700px)

> **ℹ️ Note:** 
> 
> You will connect the other end of the cable to the Farmduino in a few steps from now.
{.is-info}


# Step 3: Connect the Water Tube

Push the **water tube** onto the [M5 barb](M5 barb) on top of the [UTM](UTM) that is closest to the [z-axis extrusion](z-axis extrusion).

![utm water tube connection](/assembly/tools/_images/utm_water_tube_connection.png =700x)

> **ℹ️ Note:** 
> 
> You will connect the vacuum pump tube in a few steps from now.
{.is-info}


# What's next?

 * [Camera](camera.md)
