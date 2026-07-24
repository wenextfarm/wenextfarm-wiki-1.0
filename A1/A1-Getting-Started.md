---
title: A1 Getting Started & Configuration Guide (Important)
description: 
published: true
date: 2026-07-24T03:14:26.582Z
tags: 
editor: markdown
dateCreated: 2026-07-24T02:56:40.396Z
---

## Creating Your Web App Account
### Access the Website
Open a web browser and navigate to my.farm.bot.

Note: The WnextFarm web frontend is scheduled to launch before May 1, 2026 — stay tuned!

https://media/image1.jpeg{width="5.810416666666667in" height="2.863888888888889in"}

### 1.Register an Account
Fill in the following fields:

Email address

Your name

Password

Confirm password

Check the box to agree to the Terms of Service.

Click "Create Account".

Check your email inbox and click the confirmation link to verify your account.

https://media/image2.jpeg{width="4.486805555555556in" height="2.997916666666667in"}

### 2.Log In to Your Account
Sign in with your credentials to access the WnextFarm web application.

https://media/image3.jpeg{width="5.684722222222222in" height="2.504166666666667in"}

### 3.Select the FarmBot Version
Navigate to the Message Center.

Click on "Select FarmBot Version".

Choose version 1.2.

https://media/image4.png{width="5.676388888888889in" height="2.5256944444444445in"}

https://media/image5.jpeg{width="3.316666666666667in" height="2.384027777777778in"}

##  Configuring Firmware Version and Port
[IMPORTANT — Incorrect settings here will prevent your WnextFarm from connecting.]

Follow the steps below to open the Advanced Settings panel:

https://media/image6.png{width="5.608333333333333in" height="2.8152777777777778in"}

In the "Farm Machine" section, configure the following:

Setting	Value
Version	1.2
Flash Path	tty USB 0
https://media/image7.png{width="5.520138888888889in" height="2.8534722222222224in"}

##  Network Setup and Connection
This section covers how to connect your WnextFarm to your local network.

Turn on the power to your WnextFarm.

Using your phone or laptop, connect to the farmbot-xxxx WiFi network.

Open a web browser and go to setup.farm.bot or 192.168.24.1.

Select your preferred network type by tapping the corresponding icon — choose either Wired Ethernet or WiFi for wireless connection.

https://media/image8.png{width="2.5631944444444446in" height="3.1847222222222222in"}

Select the WiFi network name you wish to connect to, then tap "Next".

Note: If you don't see your network immediately, tap "SCAN" in the upper‑right corner to refresh the list.

https://media/image9.png{width="3.88125in" height="3.172222222222222in"}

Enter the WiFi network password, then press "Next".

https://media/image10.png{width="3.5256944444444445in" height="3.921527777777778in"}

Enter the email address and password you used to register your WnextFarm Web App account, then tap "FINISH".

https://media/image11.png{width="3.109027777777778in" height="4.128472222222222in"}

Setup is now complete.

WnextFarm OS will restart and automatically connect to your WiFi network and your Web App account.

https://media/image12.jpeg{width="3.5125in" height="4.211805555555555in"}

Reconnect your phone or computer to your regular WiFi network.

## Connection Status and Initial Setup
### 1.Access the Web App
Open your browser and go to my.farm.bot, then log in to your account.

### 2.Check Connection Status
Click the Connection Status button to verify whether your WnextFarm is properly connected to the web application.

Note: Please be patient — it may take up to 5 minutes after completing network configuration for the machine to fully restart.

https://media/image13.jpeg{width="5.422916666666667in" height="2.829861111111111in"}

If you see a red indicator for the Raspberry Pi or Arduino connection, don't worry — you may not have configured the port yet. Follow the steps below to resolve this:

Open the Advanced Settings panel as shown:

https://media/image6.png{width="5.533333333333333in" height="2.777083333333333in"}

In the "Farm Machine" section, set:

Setting	Value
Version	1.2
Flash Path	tty USB 0
https://media/image14.png{width="5.44375in" height="2.776388888888889in"}

### 3.Basic Machine Configuration
[IMPORTANT — Incorrect settings here may prevent your WnextFarm from operating properly.]

Open the Advanced Settings panel.

#### 1.1 Axes Configuration
In the "Axes" tab, set the following axis lengths:

Axis	Length
X‑axis	800 mm
Y‑axis	500 mm
Z‑axis	300 mm (adjust later using the Z‑axis limit block)
Spare soil height: -300

https://media/image15.png{width="5.391666666666667in" height="3.290277777777778in"}

#### 1.2 Encoder Settings
In the "Encoders" tab, turn off the encoders for the X, Y, and Z axes (one by one).

https://media/image16.png{width="5.377777777777778in" height="3.276388888888889in"}

#### 1.3 Limit Switch Settings
In the "Limit Switches" tab, turn on the limit switches for the X, Y, and Z axes.

https://media/image17.png{width="5.628472222222222in" height="3.6416666666666666in"}

## Adding Peripherals
### 1.Open the Peripherals Panel
Click the "Controls" button, select the Peripherals window, then click "Edit".

https://media/image18.png{width="5.374305555555556in" height="3.9243055555555557in"}

### 2.Add a New Peripheral
Click the "+" button to add a new controlled peripheral device.

https://media/image19.png{width="4.903472222222222in" height="3.29375in"}

### 3.Configure Peripherals
Add the following peripherals according to the table:

|Peripheral	|Pin	    |Signal Mode|
|-----------|---------|-----------|
|Vacuum Pump|	Pin 7   |	Digital   |
|LED        |	Pin 8	  |Digital    |
|Water Pump	|Pin 9   	|Digital    |
|Grow Light |	Pin 10	|Digital    |

https://media/image20.png{width="4.929861111111111in" height="2.589583333333333in"}

### 4.Save
Click "Save" to confirm your settings.

## Adding Tool Slots
Select the "Tools" option from the menu.

Click the "+" button in the upper‑right corner to add a new tool.

https://media/image21.png{width="4.540972222222222in" height="1.7333333333333334in"}

Select the required tools from the list:

Watering nozzle

Seeder

Weeder

Soil sensor

Seed bin

Click "+ Selected" to confirm.

https://media/image22.png{width="4.763888888888889in" height="2.5215277777777776in"}

Click "+ Add Slot" to add a tool slot.

Note: To set the slot coordinates, you will need to manually move the tool head to a position directly above the slot where it can properly dock with the tool.

https://media/image23.png{width="4.05in" height="2.966666666666667in"}

Add the remaining 4 slots in the same manner.

Note: For the remaining slots, the X and Z coordinates are identical to the first slot, while the Y‑axis spacing is 100 mm apart.

https://media/image24.png{width="4.801388888888889in" height="2.8666666666666667in"}

Based on your actual tool installation locations, assign the appropriate tool to each slot.

https://media/image25.png{width="4.759027777777778in" height="2.2333333333333334in"}

Example of completed configuration:

https://media/image26.png{width="4.815972222222222in" height="3.1118055555555557in"}

## Adding Sensors
Select the "Sensors" option from the menu.

Click the "Edit" button in the upper‑right corner.

https://media/image27.png{width="5.313194444444444in" height="2.1597222222222223in"}

Click "+" to add a new sensor.

https://media/image28.png{width="5.259027777777778in" height="2.5861111111111112in"}

Add the following sensors according to the table:

|Sensor	    |Pin     	|Signal Mode|
|-----------|---------|-----------|
|Soil Sensor|Pin 59 (A5)|	Analog|
|Tool Verification|	Pin 8|Digital|
|Vacuum Pressure Sensor|Pin 65 (A11)	|Analog|
|Light Sensor	|Pin 66 (A12)	|Analog|

Click "Back" to return.

Congratulations!
You have successfully completed the initial setup and configuration of your WnextFarm A1. You are now ready to explore and make full use of your device.

For more detailed software documentation, please refer to:

FarmBot Official Documentation (English):
https://software.farm.bot/v15/docs/intro

