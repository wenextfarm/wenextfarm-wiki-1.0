---
title: Events
description: Schedule FarmBot actions :calendar: :white_check_mark: [Open this panel in the app](https://my.farm.bot/app/designer/events)
published: true
date: 2026-07-13T06:23:29.556Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T07:53:14.398Z
---

It would not be convenient for you to manually initiate sequences every time you want them to execute. This is where **events** come in to help. If you've ever used a calendar application before, you'll feel right at home with this. Let's get started

<iframe class="embedly-embed" src="//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2Fvwnsr8zelaY%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3Dvwnsr8zelaY&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2Fvwnsr8zelaY%2Fhqdefault.jpg&key=02466f963b9b4bb8845a05b53d3235d7&type=text%2Fhtml&schema=youtube" width="854" height="480" scrolling="no" frameborder="0" allowfullscreen></iframe>

# Creating events

Navigate to the events panel on the farm designer page and press the <span class="fb-button fb-yellow"><i class='fa fa-plus'></i></span> button to create a new **event**. Choose the **SEQUENCE OR REGIMEN** that you would like to execute and provide a **START** date and time. By default, the current date and current time + 3 minutes will be input into the date and time fields.

Optionally, sequence events can be set to **REPEAT EVERY** custom interval **UNTIL** a stop date and time.

> **ℹ️ Note:** 
> 
> New events must be scheduled at least one minute into the future.
{.is-info}


> **⚠️ FarmBot performs updates at 3AM:** 
> 
> Avoid scheduling any events between 2AM and 4AM.
{.is-warning}


![events panel](/web/web-apps/_images/events_panel.png =700x)

If the sequence or regimen you selected has an [externally defined variable](sequences/externally-defined-variables.md), you will need to provide a value for that variable in the event creation panel.

![add new event panel](/web/web-apps/_images/add_new_event_panel.png =700x)

Once you are finished, press the <span class="fb-button fb-green">SAVE</span> button to save the event. The event will now show up in the agenda.

![events panel with events](/web/web-apps/_images/events_panel_with_events.png =700x)

# Editing events

To edit an event, hover over an event in the agenda view and press the <i class='fa fa-edit'></i> icon. Make the desired changes and press <span class="fb-button fb-green">SAVE</span>.

> **⚠️ Some changes aren't allowed:** 
> 
> You cannot change from executing a sequence to executing a regimen or vice versa.
{.is-warning}


![edit event button](/web/web-apps/_images/edit_event_button.png =700x)

# Deleting events

To delete an event, click on it to open up the edit event panel. Then press the <span class="fb-button fb-red">DELETE</span> button.

# What's next?

 * [Controls](controls.md)
