---
layout: page
title: Smart-Medibox
description: Smart Medibox is a EPP32 based device designed to assist users in managing their medication effectively. It integrates several features to ensure medication adherence and proper storage conditions.
img: assets/img/medibox/thumb.png
importance: 4
category: hardware
tags : ['esp32', 'iot', 'medibox']
github: https://github.com/eshansurendra/Smart-MediBox
---

> For detailed documentation and source code, visit my [GitHub Repository](https://github.com/eshansurendra/Smart-MediBox).

### Project Overview

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/medibox/overview.svg" title="Overview" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Features

1. **Medication Reminders**: The device reminds users to take their medication at specified times through alarms.

2. **Temperature and Humidity Monitoring**: Continuous monitoring of temperature and humidity inside the Medibox ensures that medications are stored under optimal conditions. Users are notified if conditions deviate from the desired range.

3. **Light Control**: A motorized curtain controls the amount of light entering the Medibox, helping to maintain the appropriate environment for medication storage.

### Technologies and Components

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/medibox/diagram.png" title="Technologies and Components" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

#### Components:
- ADAFRUIT SSD 1306 OLED Monochrome Display (128x64)
- ESP32 Devkit V1
- DHT11 Temperature and Humidity Sensor (Configurable for DHT22)
- SG90 Micro Server Motor
- LDRs and 10kΩ Resistors
- Push Buttons

### Node-RED Dashboard

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/medibox/dashboard.png" title="Node-RED Dashboard" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
