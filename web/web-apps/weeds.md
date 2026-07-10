---
title: "Weeds"
description: "Manage the weeds found in your garden [Open this panel in the app](https://my.farm.bot/app/designer/weeds)"
published: true
date: 2026-07-10T14:00:00.000Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T13:58:00.000Z
---
The **weeds panel** allows you to manage the weeds in your garden. Weeds are divided into three categories:

  * **PENDING** weeds have been [detected by FarmBot's camera](photos/weed-detection.md) and are awaiting manual triage. The <span class="fb-button fb-green"><i class='fa fa-check'></i></span> and <span class="fb-button fb-green"><i class='fa fa-check'></i> ALL</span> buttons will move weeds to the **ACTIVE** category while the <span class="fb-button fb-red"><i class='fa fa-times'></i></span> and <span class="fb-button fb-red"><i class='fa fa-times'></i> ALL</span> buttons will delete the weeds.
  * **ACTIVE** weeds are weeds currently active in the garden. These weeds were either identified by FarmBot's camera and then triaged into this category, or they were manually added with the <span class="fb-button fb-red"><i class='fa fa-plus'></i></span> button.
  * **REMOVED** weeds are weeds that are no longer a concern. This category should include weeds that have been removed by FarmBot or by hand.

![weeds panel](_images/weeds_panel.png =700px)

# Adding weeds
To manually add a weed, click the <span class="fb-button fb-red"><i class='fa fa-plus'></i></span> button in the weeds panel. This will open the **add weed** panel where you can provide a **NAME**, **COLOR**, **X**, **Y**, and **Z** coordinates, and a **RADIUS** for the weed. You can also click and drag in the map to define the coordinates and radius. Click <span class="fb-button fb-green">SAVE</span> to save the weed.

![add new weed](_images/add_new_weed.png =700px)

# Editing weeds
To edit a weed, click it in the panel or in the map (when the weeds panel is opened). This will open the **edit weed** panel, allowing you to change anything about the weed. Changes will be saved when you press the <i class='fa fa-arrow-left'></i> button.

![weeds panel with weed hovered](_images/weeds_panel_with_weed_hovered.png =700px)

# Moving to a weed
There are two ways to move FarmBot to a weed. The first way is by clicking <span class="fb-button fb-gray">MOVE DEVICE TO LOCATION</span> from the edit weed panel.

![edit weeds panel with move to weed button](_images/edit_weeds_panel_with_move_to_weed_button.png =700px)

The second way is from sequences. Simply select the weed from the **LOCATION** dropdown in a <span class="fb-step fb-move">Move</span> command or location variable.

![move to weed location step](_images/move_to_weed_location_step.png =700px)

# Deleting weeds
To delete a weed, click on it to open up the edit weed panel. Then press the <span class="fb-button fb-red">DELETE</span> button.

> **ℹ️ Note:** Weeds cannot be deleted if they are still in-use by any sequences.

# What's next?

 * [Points](points.md)
