---
title: High Level Overview
description: 
published: true
date: 2026-07-25T06:32:51.752Z
tags: 
editor: markdown
dateCreated: 2026-07-09T03:36:45.301Z
---

**WenextFarm P1** and **P1 MAX** are primarily constructed from V-slot aluminum extrusions and aluminum plates and brackets. They are driven by four NEMA 17 stepper motors with closed‑loop encoders, along with three limit switches, the MKS Gen v1.0 electronics board, and a Raspberry Pi 3 computer.  Current models cover growing areas as small 1m<sup>2</sup> up to a maximum of 18m<sup>2</sup>, and plants as tall as 1m.

![wenextfarm-p1.jpg](/wiki/wenextfarm-p1.jpg)

![wenextfarm-p1-max.jpg](/wiki/wenextfarm-p1-max.jpg)

> **Not your typical product:** 
> 
> WenextFarm is engineered to be durable, easily assembled and modified with everyday tools, and fully upgradeable. It is a refined evolution of the open‑source FarmBot — improved for practicality, reliability, and flexibility, with none of the proprietary lock‑in or planned obsolescence you might find elsewhere.
{.is-success}


At WenextFarm, we believe in the power of openness and creativity. That's why we've taken the open‑source foundation of FarmBot and refined it into a smarter, more adaptable farming companion — one that's built to be tinkered with, upgraded, and truly owned.

Whether you want to extend your tracks, design custom tools, or program your WenextFarm to do something entirely unexpected — the only limit is your imagination. Grow vegetables on your balcony, mushrooms in your basement, or flowers on a vertical wall. Experiment, fail, improve, repeat. That's the maker spirit, and it's at the heart of everything we do.

We've designed WenextFarm to be more than just a machine — it's a platform for your creativity. And we can't wait to see what you'll build with it.

Ready to get started? Our documentation is here to guide you every step of the way. And if you ever have questions, ideas, or just want to share your latest project, come join our [community forum](http://forum.wenextfarm.com). We're all ears. Cheers! 🍻

# Architecture

![结构图-压缩.jpg](/assembly/intro/_images/结构图-压缩.jpg =700x)

## Tracks
The track system sets WenextFarm apart from conventional wheeled farming equipment. It enables precise positioning with a simple, efficient mechanical design. Key advantages include:

1. High positional accuracy with consistent repeatability
2. Support for any planting layout or crop arrangement
3. Minimal footprint and no soil compaction — preserving soil health

## Gantry
The gantry bridges the two parallel tracks and moves along the X‑axis via a belt‑and‑pulley drive. It also serves as a linear guide for the cross‑slide (Y‑axis motion) and provides a mounting platform for sensors, electronics, or custom attachments.

## Cross‑slide
The cross‑slide travels along the gantry in the Y‑axis direction, providing the second degree of freedom. This enables operations such as seeding, watering, and weeding at any point within the X/Y planting plane. It is driven by a belt‑and‑pulley system and serves as the base for the Z‑axis assembly.

## Z‑axis
The Z‑axis attaches to the cross‑slide and delivers vertical motion — the third degree of freedom. It mounts the universal tool mount (UTM), allowing the WenextFarm to pick up and use a variety of interchangeable tools for different tasks.

# Economies of scale

The larger your WenextFarm, the lower the cost per square meter of growing area. For the best return on investment, we recommend installing the largest model that your space allows.

*Note that the costs below do not account for [supporting infrastructure](../supporting-infrastructure.md), which will also increase in cost as the device size increases.*

|Model  |Track Length|Gantry Width|Growing Area     |Cost    |
|-------|------------|------------|-----------------|--------|
|P1     |3m          |1.5m        |4.5m<sup>2</sup> |~$1,499 |
|P1 MAX |6m          |3m          |18m<sup>2</sup>  |~$2,399 |
