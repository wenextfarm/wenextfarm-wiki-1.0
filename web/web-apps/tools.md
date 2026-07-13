---
title: Tools
description: Manage tools and seed containers :hammer:  [Open this panel in the app](https://my.farm.bot/app/designer/tools)
published: true
date: 2026-07-13T06:42:01.937Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T07:56:42.329Z
---

On the **tools panel** you can manage all of your FarmBot's **slots**, **tools**, and **seed containers** as well as view the currently mounted tool.

> **ℹ️ Note:** 
> 
> Only Genesis kits have interchangeable tools, and the user interface may look slightly different depending on which kit you have.
{.is-info}


![tools panel](/web/web-apps/_images/tools_panel.png =700x)

# Slots

**Slots** are locations within FarmBot's coordinate system that can hold a **tool** or **seed container** and correspond to physical hardware such as a toolbay (Genesis kits) or the gantry-mounted seed trough holder (all kits).

![slot in map](/web/web-apps/_images/slot_in_map.png =700x)

## Creating slots

To create a new slot, press the <span class="fb-button fb-gray"><i class='fa fa-plus'></i></span> button next to the **SLOTS** label in the tools panel.

![add new slot](/web/web-apps/_images/add_new_slot.png =700x)

Next, provide **coordinates** for the tool slot. To input accurate coordinates, use the manual controls to move FarmBot into the target position and then click the **USE CURRENT LOCATION** <span class="fb-button fb-blue"><i class='fa fa-crosshairs'></i></span> button to copy FarmBot's current coordinates into the **X**, **Y**, and **Z** input fields.

Different tools and seed containers will require different coordinates for the slot:

  * **Interchangeable tools** (Genesis kits only) - Use coordinates for when FarmBot's UTM will fully mount the tool while it is still in the slot.
  * **Seed bins** and **seed troughs** - Use coordinates for when FarmBot's seed injector needle will be positioned to pick up a seed from the container.
  * **Seed trays** (with 16 individual cells) - Use coordinates for when FarmBot's seed injector needle is positioned between cells **A2** and **A3**, approximately 1mm above the top of the seed tray. If your tool slot’s pullout direction is in the Negative X direction, position the needle exactly between cells **D2** and **D3**. In either case, the UTM’s main cylindrical section should be aligned with the outer cylindrical face of the seed tray as in the example image below. Then use the [Pick from Seed Tray](https://my.farm.bot/app/shared/sequence/32) featured sequence for picking up seeds from a specific cell in the tray.

![seed tray setup](/web/web-apps/_images/seed_tray_setup.png =700x)

### Changing slot direction

Some slots (such as the toolbays included with Genesis kits) have a **slot direction**, which is the direction that the tool must be loaded and unloaded from. To specify a slot's direction, use the **SLOT DIRECTION** dropdown.

### Gantry-mounted slots

Some slots (such as those provided by the seed trough holder) are **gantry-mounted** and move with the FarmBot along the x-axis. To account for this and properly render these types of slots in the farm designer, you can specify that a slot is **GANTRY-MOUNTED** with a checkbox. Doing so will display the **X** coordinate as <span class="fb-input fb-disabled-input">Gantry</span>.

## Loading slots

To load a tool or seed container into the slot, select one from the **TOOL OR SEED CONTAINER** dropdown and then press <span class="fb-button fb-green">save</span>.

> **✅ IMPORTANT: The virtual configuration must match real life:** 
> 
> Now that you have **virtually** loaded your slots, you must also load the **real** tools and/or seed containers into the **real** slots to match your **virtual** configuration. If you do not do this, FarmBot may perform undesirably. And don't forget: if you change things up in real life (remove a seed bin, for example), you must update the virtual configuration to match.
{.is-success}


![profile view of tools in toolbays](/web/web-apps/_images/profile_view_of_tools_in_toolbays.png =700x)

## Deleting slots

To delete a slot, select it from the **SLOTS** list in the main tools panel and then press the <span class="fb-button fb-red">DELETE</span> button.

> **ℹ️ Note:** 
> 
> You cannot delete slots with tools or seed containers that are used in sequences.
{.is-info}


# Tools and seed containers

## Creating tools and seed containers

To create a new **tool** or **seed container**, press the <span class="fb-button fb-gray"><i class='fa fa-plus'></i></span> button. Provide a **NAME** to define the tool or seed container and then press <span class="fb-button fb-green">SAVE</span>. Alternatively, you can select from the available **STOCK NAMES** to add one or more of the standard tools and seed containers included with your FarmBot kit.

![add new tool](/web/web-apps/_images/add_new_tool.png =700x)

## Editing tools and seed containers

To edit a tool or seed container, click it from the **TOOLS AND SEED CONTAINERS** list (Genesis), or the **SEED CONTAINERS** list (Express) located at the bottom of the main tools panel. Make your desired edits and then press the <span class="fb-button fb-green">SAVE</span> button.

## Deleting tools and seed containers

To delete a tool or seed container, click it from the **TOOLS AND SEED CONTAINERS** list (Genesis), or the **SEED CONTAINERS** list (Express) located at the bottom of the main tools panel. Then click the <span class="fb-button fb-red">DELETE</span> button.

> **ℹ️ Note:** 
> 
> You cannot delete a tool or seed container if it is currently loaded into a tool slot.
{.is-info}


# What's next?

 * [Message Center](intro/message-center.md)
