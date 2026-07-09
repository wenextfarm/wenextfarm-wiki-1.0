---
title: Camera Cable
description: 
published: true
date: 2026-07-08T10:00:12.808Z
tags: 
editor: markdown
dateCreated: 2026-07-08T09:58:30.747Z
---
**Component tests**{:.internal}

|Test         |Description  |Target       |Tolerance    |
|-------------|-------------|-------------|-------------|
|Length       |Measure the length of the cable using a measuring tape.|See BOM spec|+/- 20mm
|Diameter     |Measure the diameter of the cable using digital calipers.|5mm|+/- 0.5mm
|Cable        |Inspect the spec of the cable.|Shielded 28AWG/1p + 24AWG/2c<br><br>1p = 1 twisted pair (for data)<br>2c = 2 core (for power)|N/A
|Color        |Inspect the color of the cable.|Black|N/A
|Labels       |Inspect both ends for labels.|Should be labeled "CAM"|N/A
|Function     |Use the camera cable to connect a camera to a Raspberry Pi. Take a photo using the web app.|Image should be captured as expected|N/A
|90 degree connector|Connect the 90 degree connector to a camera and submerge into a cup of water. Take a photo using the web app.|The connector should make a waterproof connection, allowing an image to be captured as expected|N/A
|Electronics box fit|Connect the camera cable to the Raspberry Pi in a fully assembled electronics box.|Cable and connector should fit|N/A
