---
title: "FarmBot OS"
description: "Step-by-step instructions for installing FarmBot OS. Download the latest FarmBot OS `.img` file at [os.farm.bot](http://os.farm.bot)."
published: true
date: 2026-07-10T14:00:00.000Z
tags: v15
editor: markdown
dateCreated: 2026-07-10T13:58:00.000Z
---
The Raspberry Pi runs a custom operating system named **FarmBot OS**, allowing FarmBot to:

  * Communicate with the web application over WiFi or ethernet so that it can synchronize (download) sequences, regimens, farm designs, events, and more; upload logs and sensor data; and accept real-time commands.
  * Communicate with the Farmduino to send G and F commands and receive sensor and encoder data.
  * Take photos with a USB or Raspberry Pi camera, and upload the photos to the web application.
  * Get configured over WiFi, mitigating the need to plug in a mouse, keyboard, or screen.

<iframe class="embedly-embed" src="//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2F76ZwipJ3Dpw%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3D76ZwipJ3Dpw&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2F76ZwipJ3Dpw%2Fhqdefault.jpg&key=02466f963b9b4bb8845a05b53d3235d7&type=text%2Fhtml&schema=youtube" width="854" height="480" scrolling="no" frameborder="0" allowfullscreen></iframe>

# Step 1: Download FarmBot OS

Using a desktop computer or laptop, go to [os.farm.bot](http://os.farm.bot) to download the latest FarmBot OS `.img` file according to your **FarmBot kit** and it's **internal computer**.

![download farmbot os](_images/download_farmbot_os.png =700px)

# Step 2. Write FarmBot OS onto the microSD card

To write FarmBot OS onto the microSD card, you must use a special **`.img` writing tool** called **[Raspberry Pi Imager](https://www.raspberrypi.com/software/)**.

> **🚫 Drag and drop will not work:** Using your computer's default file browser to drag and drop or copy and paste the FarmBot OS `.img` file onto the microSD card **will not work**. You *must* use Raspberry Pi Imager.

![raspberry pi imager](_images/rpi_imager.png =700px)

Once you have Raspberry Pi Imager installed, connect the microSD card to your computer using a **card reader**. You may need to use the **microSD card to SD card adapter** included with your kit.

Open up the Raspberry Pi Imager program and make the following selections:

1. **Raspberry Pi Device** - You do not need to click the `CHOOSE DEVICE` button nor make a selection. Your device has already been determined by the version of FarmBot OS you downloaded.
2. **Operating System** - Click `CHOOSE OS` and then scroll to the bottom of the popup and select **Use custom** _Select a custom .img file from your computer._ Then select the FarmBot OS `.img` file you downloaded in Step 1.
![select the use custom .img file in raspberry pi imager](_images/rpi_imager_use_custom_os.png =700px)
3. **Storage** - Click `CHOOSE STORAGE` and then select the microSD card (it should show up as a `7.9 GB` option).
![choose the microSD card storage](_images/rpi_imager_choose_storage.png =700px)

> **⚠️ Do not use large capacity microSD cards:** FarmBot OS will not work with microSD cards larger than 32GB in capacity. Please use the microSD card provided with your FarmBot kit.

Click `NEXT`. You will then be prompted if you would like to use OS customization settings. Select `NO`.

![no customization](_images/rpi_imager_no_customization.png =700px)

A final warning popup will be shown. Proceed to write the OS to the microSD card. Your computer may ask you for permission to perform this action. Once permission is granted, Raspberry Pi Imager will write FarmBot OS to the microSD card and then verify the installation. The process will take approximately 1 minute.

![raspberry pi imager writing](_images/rpi_imager_writing.png =700px)

After completing, you may remove the microSD card from your computer and close Raspberry Pi Imager.

![raspberry pi imager complete](_images/rpi_imager_complete.png =700px)

# Step 3. Insert the microSD card into the Raspberry Pi

Insert the **microSD card** into the **Raspberry Pi**. The card slot location will differ depending on the FarmBot kit you have.

## Genesis kits

For Genesis kits, the card slot is located on the back side of the Raspberry Pi, on the right-hand edge. You do not need to remove the Raspberry Pi from the electronics box to insert the card; we have left enough access room.

![MicroSD card slot on the Raspberry Pi 3](_images/microsd_card_slot_on_the_raspberry_pi_3.jpeg =700px)

## Express kits

For Express kits, the card slot is located on the front side of the Raspberry Pi, on the left-hand edge.

![MicroSD card slot on the Raspberry Pi Zero W](_images/microsd_card_slot_on_the_raspberry_pi_0.jpeg =700px)

# Step 4. Plug in the power source

Plug your FarmBot's power supply into a wall outlet. You should now see a solid red <span class="fa fa-circle red"></span> LED and a steadily flashing green <span class="fa fa-circle led green"></span> LED on the Raspberry Pi, indicating that the Pi has adequate power and is busy booting up. Refer to the [status LEDs](intro/status-leds.md) page for more information, especially if your LEDs are not lit up as described above.

# What's next?

 * [Configurator](intro/configurator.md)
 * [Status LEDs](intro/status-leds.md)
 * [Data Usage](intro/data-usage.md)
 * [Auto Updates](intro/auto-updates.md)
