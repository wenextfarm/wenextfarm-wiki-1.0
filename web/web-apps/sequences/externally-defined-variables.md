---
title: Externally Defined Variables
description: 
published: true
date: 2026-07-13T06:17:27.654Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T08:03:02.223Z
---

There are five places that you can provide a value for an **externally defined variable**:
1. When using the [run button](#run-button)
2. In an [execute step](#execute-step)
3. In a [parent sequence's header](#parent-sequence-header)
4. In a [regimen header](#regimen-header)
5. In an [event](#event)

When providing the variable value in any of these places, you will be initially presented with the variable's **DEFAULT VALUE**, which may serve as a shortcut when set to a frequently used value.

# Run button

If you want to test run your sequence, you will need to provide a value for the variable to be used during the run. Simply click the <span class="fb-button fb-orange">RUN</span> button and provide a variable value in the popup form. Then click <span class="fb-button fb-orange">RUN</span> again and FarmBot will execute the sequence with the variable value provided. You can test run your sequence as many times as you want with the same or different variable values each time.

![run button variables](/web/web-apps/sequences/_images/run_button_variables.png =700x)

# Execute step

If you add your sequence to another sequence using an <span class="fb-step fb-execute">EXECUTE</span> command, then a variable form will be shown in the step.

![execute with variable](/web/web-apps/sequences/_images/execute_with_variable.png =700x)

# Parent sequence header

If you add your sequence to another sequence using an <span class="fb-step fb-execute">EXECUTE</span> command, you may select **Variables** - `Add new` to add a *new variable* that belongs to the parent sequence. You can then provide a value for that variable in the sequence header, and it will be passed into the subsequence(s). Notice that the value you choose will be displayed in each <span class="fb-step fb-execute">EXECUTE</span> command that the value will be passed into.

![pass variable value from parent to subsequences](/web/web-apps/sequences/_images/pass_variables.png =700x)

> **ℹ️ Russian doll sequences:** 
> 
> By setting the new variable in the parent sequence to `Externally defined`, you can create a set of \
{.is-info}


# Regimen header

If you add your sequence to a regimen, then a variable form will be shown in the regimen's header. You can provide a value right there, or choose `Externally defined`, in which case you will need to provide a value in the event that runs the regimen (see below). All regimen items will show the variables and the values that will be used when the sequence is run (either the explicitly set values in the regimen, or the variable’s default values).

![regimen variable form](/web/web-apps/sequences/_images/regimen_variable_form.png =700x)

# Event

If you make an event for a sequence or a regimen with a variable set to `Externally defined`, then a variable form will appear in the add event panel.

![event variable form](/web/web-apps/sequences/_images/event_variable_form.png =700x)

Once the event has been scheduled, all event instances will show the variables and the values that will be used when the event runs (either the explicitly set values in the event or the variable’s default values).

![variable values in event instance](/web/web-apps/sequences/_images/variable_values_in_event.png =700x)

# What's next?

 * [Multiple Variables](multiple-variables.md)
