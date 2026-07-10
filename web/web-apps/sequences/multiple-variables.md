---
title: "Multiple Variables"
description: "Using more than one variable in a sequence"
published: true
date: 2026-07-10T14:00:00.000Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T13:58:00.000Z
---
# Adding multiple variables

Sequences are not limited to a single variable. To add additional variables click the <span class="fb-button fb-gray"><i class='fa fa-plus'></i></span> button in the **VARIABLES** section of the sequence editor, followed by the <span class="fb-button fb-gray">variable type</span> desired or select `Add new` in a sequence step dropdown.

![add multiple variables](_images/add_multiple_variables.png =700px)


# Removing variables

To remove a variable, click the <i class='fa fa-trash'></i> icon.

> **ℹ️ Note:** Only unused variables can be removed.

![remove variable](_images/remove_variable.png =700px)

# Renaming variables

To keep track of what each variable is used for, click the variable's title to add a custom name.

> **ℹ️ Note:** Variables cannot be renamed once in-use by sequence commands, so do the naming up-front.

![rename variable](_images/rename_variables.png =700px)

# Multiple externally defined variables

All `Externally defined` variables will be displayed in the run button popup, execute steps, and all other places where you can provide a value for an [externally defined variable](externally-defined-variables.md).

![multiple variable run button](_images/multiple_variable_run_button.png =700px)

> **⚠️ Only one group variable is allowed per sequence:** When FarmBot runs a sequence with a group variable, it will actually execute the sequence multiple times - once for each member of the group. If a sequence had more than one group variable, it would not be clear what order FarmBot should execute the sequence in. Thus, at this time, multi-group execution is not allowed.

# What's next?

 * [Variable Types](variable-types.md)
