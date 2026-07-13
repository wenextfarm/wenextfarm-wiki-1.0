---
title: Sensors
description: Manually read FarmBot's sensors 🌡️ [Open this panel in the app](https://my.farm.bot/app/designer/sensors)
published: true
date: 2026-07-13T06:29:08.503Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T08:02:24.932Z
---

The **sensors panel** allows you to manage FarmBot's sensors, take measurements, and view historical sensor readings.

> **ℹ️ Not shown for all bots:** 
> 
> If your FarmBot kit did not include any sensors (Express kits), then the sensors panel will not be shown in the app. You can override this using the **HIDE SENSORS** setting.
{.is-info}


![sensors panel](/web/web-apps/controls/_images/sensors_panel.png =700x)

# Creating sensors

To create a new sensor, press <span class="fb-button fb-gray">EDIT</span>, and then the <span class="fb-button fb-green"><i class='fa fa-plus'></i></span> button. To define the sensor, provide a <span class="fb-input">Name</span>, choose a <span class="fb-dropdown">Pin #</span>, and specify if the sensor is `Digital` or `Analog`. Pressing <span class="fb-button fb-green"><i class='fa fa-plus'></i> STOCK SENSORS</span> will add all of the standard sensors included with your FarmBot kit.

> **⚠️ Note:** 
> 
> Pin numbers are required and must be unique.
{.is-warning}


When finished editing, press <span class="fb-button fb-green">SAVE</span>.

![edit sensors](/web/web-apps/controls/_images/edit_sensors.png =700x)

# Reading sensors

To manually read a sensor, press its <span class="fb-button fb-gray">READ SENSOR</span> button. FarmBot will then read the sensor and display the value next to the sensor name. Digital sensors will provide a value of either `0` or `1`, while analog sensors will provide a value between `0` and `1023`.

![read sensors](/web/web-apps/controls/_images/read_sensors.png =700x)

You can also read sensors from [sequences](sequences.md) by using the <span class="fb-step fb-read-pin">READ SENSOR</span> command. For more information, see the [read sensor command documentation](sequences/sequence-commands/peripherals-and-sensors.md#read-sensor).

## Historical readings

Use the **SENSOR HISTORY** section of the panel to view sensor readings from the past. Optionally, you can filter by **SENSOR**, **TIME PERIOD**, and/or **X**, **Y**, and **Z** coordinates. The **DEVIATION** field can be used to filter within a range of locations around the specified coordinates. To remove all current filters, press <span class="fb-button fb-gray">CLEAR FILTERS</span>.

![sensor reading history](/web/web-apps/controls/_images/sensor_reading_history.png =700x)

## Manual readings

You can track custom garden metrics over time without the use of a physical sensor connected to your FarmBot's electronics by manually adding sensor readings. For example, you could create a sensor named "Frost days" and every day that you experience frost at your garden site, manually add a corresponding reading.

To manually add a sensor reading, click the <span class="fb-button fb-green"><i class='fa fa-plus'></i></span> button, enter the reading details, and press <span class="fb-button fb-green">SAVE</span>.

![add manual sensor reading](/web/web-apps/controls/_images/add_manual_sensor_reading.png =700x)

# Deleting sensors

To delete a sensor, press <span class="fb-button fb-gray">edit</span> and then the sensor's <span class="fb-button fb-red"><i class='fa fa-times'></i></span> button. Finish editing by pressing <span class="fb-button fb-gray">back</span>.

> **ℹ️ Note:** 
> 
> You cannot delete a sensor that is in-use by a sequence.
{.is-info}


# Hiding sensors

If you do not plan to use any sensors, use the **HIDE SENSORS** toggle in the [app settings panel](settings/account-settings.md) to remove the sensors panel.


# What's next?

 * [Photos](photos.md)
