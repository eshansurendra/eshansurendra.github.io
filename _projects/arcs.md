---
layout: page
title: Automatic Retractable Clothesline System
description: Arduino-based project designed to simplify the process of drying clothes outdoors. By incorporating various sensors and a stepper motor, the system can automatically retract the clothesline in response to rain or adverse weather conditions.
img: assets/img/arcs/team.png
importance: 1
category: hardware
tags : ['arcs', 'arduino', 'clothsline', 'iot']
github: https://github.com/eshansurendra/Automatic-Retractable-Clothesline-System
---

> For detailed documentation and source code, visit my [GitHub Repository](https://github.com/eshansurendra/Automatic-Retractable-Clothesline-System).

> Visit our [ElectroMavericks website](https://www.electromavericks.systems/) for more details about the `Automatic Retractable Clothesline System (ARCS)`.

Automate and enhance your clothesline experience with this Arduino-based system. It automates the retraction process triggered by rain detection, protecting clothes during inclement weather. The system offers remote data monitoring via `Thingspeak` and convenient control through a `mobile app`.

### Features

- **Automated Rain Detection:** Equipped with a rain sensor, the system retracts the clothesline when rain or moisture is detected, protecting the clothes from getting wet.
- **Humidity and Temperature Monitoring:** Utilizes a DHT (Digital Humidity and Temperature) sensor to monitor ambient humidity and temperature, helping users determine the optimal time for clothes drying.
- **Light Intensity Sensing:** An LDR (Light Dependent Resistor) measures ambient light intensity. The system considers this data when deciding whether to retract the clothesline, accounting for low light conditions even if rain is detected.
- **Stepper Motor Control:** Employs a stepper motor to control the movement of the clothesline. It rotates to retract the line during adverse conditions and reverses the rotation to extend it when conditions improve.
- **Remote Monitoring with Thingspeak Integration:** Integrated with the Thingspeak platform, allowing users to remotely monitor the system's status. Real-time data, including temperature, humidity, and rain status, can be viewed through the Thingspeak web interface or mobile app.
- **Mobile App for Remote Control:** ARCS comes with a dedicated mobile app that allows you to control and monitor your Automatic Retractable Clothesline System from anywhere. The mobile app is available on `Android` platform.


### Remote Monitoring and Control

#### Thingspeak Visualization

- Access real-time data, including temperature, humidity, and rain status

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/arcs/dash.png" title="dashboard" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Check out the real-time data visualization of your ARCS system on Thingspeak. Visit [Thingspeak](https://thingspeak.com/channels/2225714) for detailed analytics and monitoring.

#### Mobile App for Remote Control

ARCS comes with a dedicated mobile app that allows you to control and monitor your Automatic Retractable Clothesline System from anywhere. The mobile app is available on [Android](#) platform.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/arcs/app.png" title="app" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

##### Features:

- **Remote Control:** Start, stop, or customize the drying process remotely.
- **Real-time Monitoring:** Monitor the status of your clothesline system, including temperature, humidity, and rain detection.
- **Notification Alerts:** Receive instant alerts on your mobile device for important events such as rain detection or system malfunctions.

##### Installation:

 -**Android:** Download the app from [Releases Section](https://github.com/eshansurendra/Automatic-Retractable-Clothesline-System/releases/tag/v1.0.0).

### Circuit Design

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/arcs/sch.png" title="sch" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/arcs/pcb3d.png" title="pcb3d.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Enclosure Design

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/arcs/enclousure.png" title="enclousure" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/arcs/pannel.png" title="pannel" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
