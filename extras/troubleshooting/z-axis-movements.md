---
title: Z-Axis Movements
description: 
published: true
date: 2026-07-09T05:41:12.505Z
tags: 
editor: markdown
dateCreated: 2026-07-09T04:07:17.114Z
---

# 1. Adjust the z-axis speed and acceleration

Try lowering the z-axis **[MAX SPEED](https://my.farm.bot/app/designer/settings?highlight=max_speed)** and **[ACCELERATE FOR](https://my.farm.bot/app/designer/settings?highlight=accelerate_for)** a longer distance. You may try halving the default max speed and doubling the default acceleration distance as a starting point, but because every FarmBot installation is a bit different, you will need to experiment to find the best values for you.

# 2. Check the z-axis eccentric spacers

Check the **eccentric spacers** on the **cross-slide** that are used to adjust the [V-wheels](V-wheels) that support the [z-axis extrusion](z-axis extrusion). If the eccentric spacers are adjusted too tightly, then they will exert too much force onto the z-axis extrusion which can make it difficult or impossible for the z-axis motor to raise the z-axis. With the FarmBot powered off, you should be able to rotate the leadscrew by hand without too much effort. If the eccentric spacers are too tight, this will be very difficult to do.

# 3. Lubricate the leadscrew

It is possible that dust and debris can build up on the [leadscrew](leadscrew) causing additional friction between the leadscrew and the [leadscrew block](leadscrew block). Clean the leadscrew with a rag and then add some lubricant which can be purchased from a local hardware store.

We recommend using a dry graphite lubricant spray which will coat the surface with a fast drying coating of graphite to create a slippery surface that reduces the resistance of movement through the leadscrew block and also may decrease any noise from the leadscrew.

We have found a product called [Jig-a-Loo Graphite Lubricant](https://www.amazon.com/dp/B08285N7LG/) that can help reduce friction on the FarmBot Z-axis leadscrew. Here is a [YouTube video](https://youtu.be/lyZ465jdO2Y) that shows how the product is used and the typical applications.

Apply enough graphite lubricant so that the hue of the screw looks significantly darker than the original silver metallic color. You should use enough graphite lubricant so that the screw should appear black or dark grey. This will allow the screw to operate without friction and vibrations. Please apply the graphite lubricant to the bottom 90% of the lead screw leaving the very top 10% unlubricated so that a sturdy grip can be applied to leadscrew by the coupler.

> **⚠️ Do not use oil, silicon, or lithium based lubricants:** These types of lubricants will attract dust and gum up causing poor performance. Only graphite lubricants are acceptable.

> **⚠️ Do not lubricate belts and pulleys:** In case you are reading this document and also have issues with movements on the X or Y axes, do not take this piece of advice (\

# 4. Adjust the stepper driver to deliver more power

For Genesis v1.5+ kits, increase the z-axis **[MOTOR CURRENT](https://my.farm.bot/app/designer/settings?highlight=motor_current)** by 100 or 200 milliamps. For v1.4 kits and below, you can adjust the **z-axis stepper driver** to deliver more power to the **z-axis motor** using the instructions at the bottom of [this post](https://forum.farmbot.org/t/why-is-my-farmbot-not-moving/2093).

# 5. Check the shaft coupler for slipping

The aluminum [shaft coupler](shaft coupler) connects the Z-axis [motor](motor) to the [leadscrew](leadscrew) to allow FarmBot to move in the Z direction up and down depending on the rotation of the motor.

Check to make sure that the shaft coupler is not slipping as it transfers rotational power from the motor to the leadscrew. If there is slipping, tighten the screws on the coupler. You may optionally use blue Loctite to prevent the screws from loosening over time.

![shaft coupler screws](_images/shaft_coupler_screws.png =700px)
