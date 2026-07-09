---
title: Seeder
description: 
published: true
date: 2026-07-08T10:00:12.808Z
tags: 
editor: markdown
dateCreated: 2026-07-08T09:58:30.747Z
---
The **seeder tool** works by using a [vacuum pump](vacuum pump) to suction-hold a single seed at the end of a **needle**.


![seeder](_images/seeder.png =700px)

> **✅ Pre-assembled for your convenience:** As of the v1.6 hardware release, the seeder tool comes [pre-assembled](../../manufacturing/pre-assembly/tools/seeder.md). In the next steps we'll hook up the rest of FarmBot's vacuum system.

# Step 1: Selecting a luer lock needle

FarmBot comes with different [luer lock needle](luer lock needle) sizes so that you can experiment and find the best needle for your needs.

|Size  |Gauge|Inner Diameter |Good for                 |
|------|-----|---------------|-------------------------|
|Large |16   |1.35mm (0.053")|Large seeds (eg: pumpkin)
|Medium|19   |0.83mm (0.032")|Most seeds
|Small |22   |0.48mm (0.019")|Small seeds (eg: lettuce)

Once you've selected a needle, attach it to the [luer lock adapter](luer lock adapter) with a quarter turn. At any time you can quickly swap the needle out for another size or replace a damaged one.

![seeder with needle](_images/seeder_with_needle.png =700px)

# Step 2: Connect the vacuum tubes and filter

> **ℹ️ Note:** For the next two steps, it can be helpful to temporarily unscrew the [vacuum pump mount](vacuum pump mount) from the [z-axis extrusion](z-axis extrusion) and slide it (and the vacuum pump) out from the housing.

Slide one of the **vacuum tubes** onto the _inlet barb_ of the [vacuum pump](vacuum pump). The inlet will be marked with an arrow pointing into the pump. The inlet may be on the left or the right side of the pump depending on when your kit was purchased. Please refer to the arrows on your pump to ensure the tube is connected correctly.

Then slide the [inline air filter](inline air filter) onto the end of the first tube and connect the second vacuum tube between the air filter and the [M5 barb](M5 barb) on top of the [UTM](UTM) closest to the FarmBot logo.

![Connect the first vacuum pump tube](_images/vacuum_tube_1.png =700px)
![Connect the inline air filter](_images/air_filter.png =700px)
![Connect the second vacuum tube](_images/vacuum_tube_2.png =700px)

> **ℹ️ Is your seeder blowing?:** If you find during testing that there is air blowing out of the seeder tool, you may try connecting the tube to the other port. We use parts from different suppliers and the vacuum pump configuration may be different on your model.

# Step 3: Wire up the vacuum pump

Connect the [z vacuum pump cable](z vacuum pump cable) to the [vacuum pump](vacuum pump) terminals according to the instructions below.


If you have the newer style cable with a single black connector, simply plug this into the vacuum pump. It will only fit in one orientation.

![Wire up the vacuum pump (single connector)](_images/wire_up_vacuum_pump_detail_new.png =700px)

If you have the older style cable with three quick-connect terminals, connect them to the vacuum pump as follows:

* Connect the **clear/silver wire** to the _terminal on the left_ labelled `PE`.
* Connect the **white wire** to the _middle terminal_ labelled `24V`.
* Connect the **black wire** to the _terminal on the right_ labelled `GND`.

If you cannot see the colors of the wires, carefully peel back the black heatshrink covering the whole cable so that you can correctly identify the individual wire colors.

![Wire up the vacuum pump](_images/wire_up_vacuum_pump_detail.png =700px)
![Wire up the vacuum pump](_images/wire_up_vacuum_pump.png =700px)

> **🚫 Double check the wiring:** Carefully inspect the images above and table below to ensure you have connected the wires correctly. **If you incorrectly wire up the vacuum pump, the vacuum pump's electronics will be permanently damaged as soon as your FarmBot is powered up.**

|Wire color  |Should be connected to
|------------|-----------------------|
|Clear/silver|`PE` (Protect Earth)
|White       |`24V` (24 Volts)
|Black       |`GND` (Ground)

# Step 4: Attach the seed trough holder

Attach the [seed trough holder](seed trough holder) to the [seed trough holder mount plate](seed trough holder mount plate) using two [M5 x 30mm screws](M5 x 30mm screws) and [M5 flange locknuts](M5 flange locknuts). Then mount the assembly to the **left gantry column** using a [40mm nut bar](40mm nut bar) and two [M5 x 10mm screws](M5 x 10mm screws).

Place the two [seed troughs](seed troughs) into the holder. Optionally, you may store up to three [luer lock needles](luer lock needles) in the holder as well.

![Attach the seed trough holder to the mount](_images/seed_trough_mount_plate.png =700px)
![Mounted seed trough holder](_images/mounted_seed_trough_holder.png =700px)

# Step 5: Understanding the seed containers


We offer the following types of seed containers, each optimized for different purposes.

## Seed bins

The [seed bins](seed bins) are for holding large amounts of one type of seed. This is best used when planting many plants of the same crop, for example: when growing microgreens. To use a seed bin, simply slide it into the **toolbay** and fill it with seeds. Then run a planting sequence from the web app with the corresponding seed bin sequence and location.

![seed bin](_images/seed_bin.jpg =700px)

If desired, you can mix a variety of seed types into one seed bin and have FarmBot plant whatever it happens to grab. Keep in mind though that FarmBot will have no way of knowing which seeds it grabs, so only use this technique when you will be taking care of all those plants identically. An example for this again might be when growing microgreens - you can grow three different types in the same area at the same time, all in the same way, without having to do three planting sequences or otherwise treat them differently.

## Seed trays

The [seed trays](seed trays) have 16 small area for holding seeds. They are best used when planting many different crops, and when the number of seeds per hole needs to be strictly controlled.

![seed trays](_images/seed_trays.jpg =700px)

## Seed troughs

The [seed troughs](seed troughs) are small seed containers that are stored in the [seed trough holder](seed trough holder), which is mounted on the gantry. This allows FarmBot to bring seeds with it along the x-axis, reducing the time to sow an entire bed.

![seed troughs](_images/seed_troughs.jpeg =700px)

# What's next?

 * [Watering Nozzle](watering-nozzle.md)
