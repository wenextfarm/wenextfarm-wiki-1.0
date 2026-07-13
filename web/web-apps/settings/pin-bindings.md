---
title: Pin Bindings
description: :radio_button: Trigger actions and sequences with physical buttons or additional sensors. [Open these settings in the app](https://my.farm.bot/app/designer/settings?highlight=pin_bindings)
published: true
date: 2026-07-13T06:54:03.205Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T07:56:24.444Z
---

> **⚠️ Note:** 
> 
> It is no longer recommended to create and manage pin bindings from the settings panel. Instead, use the [push button interface](../../app/controls/peripherals.md#push-buttons) found in the peripherals section of the controls panel.
{.is-warning}


**Pin bindings** allow electrical signals from a button or sensor to trigger a FarmBot **action** or **sequence**. For example, a red button could be used to trigger the <span class="fb-button fb-red">E-STOP</span> action as recommended with FarmBot Genesis v1.4+ and Express v1.0+ kits. For practical examples, see our [use FarmBot's buttons](../../docs/how-to-guides/use-farmbots-buttons.md) how-to guide.

# Add a pin binding for a stock button

To add a pin binding for one of the stock buttons, click the <span class="fa fa-circle-o-notch"></span> icon to open the Push Button diagram and select the button you wish to add a binding for. Then choose the **Action** or **Sequence** you would like FarmBot to take when the button is pressed. Click <span class="fb-button fb-green">SAVE</span> to save the pin binding.

![add stock pin binding](/web/web-apps/settings/_images/pin_binding.gif =700x)

# Add a pin binding for a custom GPIO pin

To add a pin binding for a custom GPIO pin, click the <span class="fa fa-th-large"></span> icon to open the GPIO diagram and select the pin you wish to add a binding for. Then choose the **Action** or **Sequence** you would like FarmBot to take when this pin goes high. Click <span class="fb-button fb-green">SAVE</span> to save the pin binding.

> **⚠️ Warning:** 
> 
> Binding to a pin without a physical button and pull-down resistor connected may put FarmBot into an unstable state.
> 
> Buttons should be connected between the selected pin and +3.3v.
{.is-warning}


# Delete a pin binding

To delete a pin binding, press the <span class="fb-button fb-red"><i class='fa fa-times'></i></span> button.
