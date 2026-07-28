---
title: A1 Getting Started & Configuration Guide (Important)
description: 
published: true
date: 2026-07-28T02:34:02.180Z
tags: 
editor: markdown
dateCreated: 2026-07-24T02:56:40.396Z
---

## Creating Your Web App Account
### Access the Website
Open a web browser and navigate to my.farm.bot.

Note: The WnextFarm web frontend is scheduled to launch before May 1, 2026 — stay tuned!

![1.jpg](/wiki/a/1.jpg =700x)

### 1.Register an Account
Fill in the following fields:

- Email address
- Your name
- Password
- Confirm password
- Check the box to agree to the Terms of Service.

Click **Create Account**.

Check your email inbox and click the confirmation link to verify your account.

![2.jpg](/wiki/a/2.jpg =700x)

### 2.Log In to Your Account
Sign in with your credentials to access the WnextFarm web application.

![3.jpg](/wiki/a/3.jpg =700x)

### 3.Select the FarmBot Version
Navigate to the Message Center.

Click on "Select FarmBot Version".

> Choose version 1.2.
{.is-success}


![4.jpg](/wiki/a/4.jpg =700x)

![5.jpg](/wiki/a/5.jpg =700x)

##  Configuring Firmware Version and Port

> IMPORTANT 
> 
> Incorrect settings here will prevent your WnextFarm from connecting.
{.is-warning}


Follow the steps below to open the Advanced Settings panel:

![6.jpg](/wiki/a/6.jpg =700x)

In the "Farm Machine" section, configure the following:

Setting	Value
Version	1.2
Flash Path	tty USB 0

![7.jpg](/wiki/a/7.jpg =700x)

##  Network Setup and Connection
This section covers how to connect your WnextFarm to your local network.

- Turn on the power to your WnextFarm.
- Using your phone or laptop, connect to the farmbot-xxxx WiFi network.
- Open a web browser and go to setup.farm.bot or 192.168.24.1.
- Select your preferred network type by tapping the corresponding icon — choose either Wired Ethernet or WiFi for wireless connection.

![图片_8.jpg](/wiki/a/图片_8.jpg =700x)

Select the WiFi network name you wish to connect to, then tap "Next".

> **Note**
> 
> If you don't see your network immediately, tap **SCAN** in the upper‑right corner to refresh the list.
{.is-info}


![图片_9.jpg](/wiki/a/图片_9.jpg =700x)

Enter the WiFi network password, then press "Next".

![图片_10.jpg](/wiki/a/图片_10.jpg =700x)

Enter the email address and password you used to register your WnextFarm Web App account, then tap "FINISH".

![图片_11.jpg](/wiki/a/图片_11.jpg =700x)

> **Setup is now complete**.
{.is-success}


WnextFarm OS will restart and automatically connect to your WiFi network and your Web App account.

![图片_12.jpg](/wiki/a/图片_12.jpg =700x)

Reconnect your phone or computer to your regular WiFi network.

## Connection Status and Initial Setup
### 1.Access the Web App
Open your browser and go to my.farm.bot, then log in to your account.

### 2.Check Connection Status
Click the Connection Status button to verify whether your WnextFarm is properly connected to the web application.

> **Note**
> 
> Please be patient — it may take up to 5 minutes after completing network configuration for the machine to fully restart.
{.is-info}

![13.jpg](/wiki/a/13.jpg =700x)

If you see a red indicator for the Raspberry Pi or Arduino connection, don't worry — you may not have configured the port yet. Follow the steps below to resolve this:

Open the Advanced Settings panel as shown:

![14.jpg](/wiki/a/14.jpg =700x)

In the "Farm Machine" section, set:

Setting	Value
Version	1.2
Flash Path	tty USB 0

![15.jpg](/wiki/a/15.jpg =700x)

### 3.Basic Machine Configuration

> **IMPORTANT**
> 
> Incorrect settings here may prevent your WnextFarm from operating properly.
> Open the Advanced Settings panel.
{.is-warning}


#### 1.1 Axes Configuration
In the "Axes" tab, set the following axis lengths:

- Axis	Length
- X‑axis	800 mm
- Y‑axis	500 mm
- Z‑axis	300 mm (adjust later using the Z‑axis limit block)
- Spare soil height: -300

![16.jpg](/wiki/a/16.jpg =700x)

#### 1.2 Encoder Settings
In the "Encoders" tab, turn off the encoders for the X, Y, and Z axes (one by one).

![17.jpg](/wiki/a/17.jpg =700x)

#### 1.3 Limit Switch Settings
In the "Limit Switches" tab, turn on the limit switches for the X, Y, and Z axes.

![18.jpg](/wiki/a/18.jpg =700x)

## Adding Peripherals
### 1.Open the Peripherals Panel
Click the "Controls" button, select the Peripherals window, then click "Edit".

![19.jpg](/wiki/a/19.jpg =700x)

### 2.Add a New Peripheral
Click the "+" button to add a new controlled peripheral device.

![20.jpg](/wiki/a/20.jpg =700x)

### 3.Configure Peripherals
Add the following peripherals according to the table:

|Peripheral	|Pin	    |Signal Mode|
|-----------|---------|-----------|
|Vacuum Pump|	Pin 7   |	Digital   |
|LED        |	Pin 8	  |Digital    |
|Water Pump	|Pin 9   	|Digital    |
|Grow Light |	Pin 10	|Digital    |

![21.jpg](/wiki/a/21.jpg =700x)

### 4.Save
Click "Save" to confirm your settings.

## Adding Tool Slots
Select the "Tools" option from the menu.

Click the "+" button in the upper‑right corner to add a new tool.

![22.jpg](/wiki/a/22.jpg =700x)

Select the required tools from the list:
- Watering nozzle
- Seeder
- Weeder
- Soil sensor
- Seed bin

Click "+ Selected" to confirm.

![23.jpg](/wiki/a/23.jpg =700x)

Click "+ Add Slot" to add a tool slot.

Note: To set the slot coordinates, you will need to manually move the tool head to a position directly above the slot where it can properly dock with the tool.

![24.jpg](/wiki/a/24.jpg =700x)

Add the remaining 4 slots in the same manner.

> **Note**
> 
> For the remaining slots, the X and Z coordinates are identical to the first slot, while the Y‑axis spacing is 100 mm apart.
{.is-warning}


![25.jpg](/wiki/a/25.jpg =700x)

Based on your actual tool installation locations, assign the appropriate tool to each slot.

![26.jpg](/wiki/a/26.jpg =700x)

Example of completed configuration:

![27.jpg](/wiki/a/27.jpg =700x)

## Adding Sensors
Select the "Sensors" option from the menu.

Click the "Edit" button in the upper‑right corner.

![28.jpg](/wiki/a/28.jpg =700x)

Click "+" to add a new sensor.

![29.jpg](/wiki/a/29.jpg =700x)

Add the following sensors according to the table:

|Sensor	    |Pin     	|Signal Mode|
|-----------|---------|-----------|
|Soil Sensor|Pin 59 (A5)|	Analog|
|Tool Verification|	Pin 63（A9）|Digital|
|Vacuum Pressure Sensor|Pin 65 (A11)	|Analog|
|Light Sensor	|Pin 66 (A12)	|Analog|

Click **Back** to return.

> **Congratulations!**
> 
> You have successfully completed the initial setup and configuration of your WnextFarm A1. You are now ready to explore and make full use of your device.
{.is-success}




> **For more detailed software documentation, please refer to**
> FarmBot Official Documentation (English):[https://software.farm.bot/v15/docs/intro](https://software.farm.bot/v15/docs/intro)
{.is-info}


