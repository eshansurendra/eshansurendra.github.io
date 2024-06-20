---
layout: page
title: Five-Band Audio Equalizer
description: Developed a fully functional audio equalizer using operational amplifier (op-amp) based active filters, enabling
 the adjustment of gains across the low, mid, and high-frequency ranges.
img: assets/img/fiveband/thumb.png
importance: 2
category: hardware
tags : ['analog', 'filters', 'opamp']
github: https://github.com/eshansurendra/FIVE-BAND-AUDIO-EQUALIZER
---

> For detailed documentation and source code, visit my [GitHub Repository](https://github.com/eshansurendra/FIVE-BAND-AUDIO-EQUALIZER).

The Five-Band Audio Equalizer project focuses on the development and implementation of a graphic equalization circuit that can manipulate audio signals across five specific frequency bands. Designed as part of the Laboratory Practice module in semester 3, this project aims to enhance hands-on skills in electronics by creating a fully functional audio equalizer using operational amplifier (op-amp) based active filters, enabling the adjustment of gains across the low, mid, and high-frequency ranges.

### Features

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/fiveband/overview.png" title="Overview Diagram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- **Adjustable Frequency Bands**: Control over five specific frequency ranges for detailed audio customization.
  - Low: 20-300Hz
  - Low Mid: 300-1kHz
  - Mid: 1kHz-4kHz
  - High Mid: 4kHz-10kHz
  - High: 10kHz-20kHz
- **Active Filtering**: Utilization of low-pass, high-pass, and band-pass filters to isolate and adjust specific frequency bands.
- **Op-Amp Circuits**: Employment of operational amplifiers for the filter circuits, ensuring high-quality signal processing.

### Tools Used

- **Circuit Design & Simulation**: Filter Pro for filter calculations and NI Multisim for circuit simulation.
- **PCB Design**: Altium Designer for creating the printed circuit board layout.
- **Enclosure Design**: SolidWorks for designing the custom enclosure.


### Circuit Design

##### Schematic Diagram

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/fiveband/EquilizerSchematicDiagram.png" title="Equilizer Schematic Diagram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

##### PCB 3D View

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/fiveband/pcb_main_3D.png" title="Equilizer PCB 3D View" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Circuit Design

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/fiveband/pcb_main_3D_2.png" title="Equilizer PCB 3D View" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Enclosure Design

The enclosure design was developed using SolidWorks, focusing on aesthetics, functionality, and durability.

#### Enclosure

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/fiveband/enclousure_assembly_view.png" title="Enclosure Design" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Demo

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/fiveband/clip.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>

