---
layout: page
title: Object-Tracking-with-SIFT-using-OpenCV
description: Implementation of object tracking using Scale-Invariant Feature Transform (SIFT) features in OpenCV with Python.
img: assets/img/sift/features.png
importance: 4
category: software
tags : ['unet', 'sementic-segmentation', 'tensorflow']
related_publications: false
github: https://github.com/eshansurendra/Object-Tracking-with-SIFT-using-OpenCV
---

> For detailed documentation and source code, visit this [GitHub Repository](https://github.com/eshansurendra/Object-Tracking-with-SIFT-using-OpenCV).

## Project Overview

This project demonstrates object tracking using Scale-Invariant Feature Transform (SIFT) features with OpenCV in Python. SIFT is a powerful feature detection algorithm that excels in identifying distinctive points in images, which are invariant to scale, rotation, and illumination changes. This capability makes SIFT particularly effective for tracking objects across video frames.

The main goal of this project is to implement and showcase object tracking using SIFT features. The method involves detecting and matching keypoints between frames to accurately track the object of interest throughout a video.

## Key Features

* Object Tracking with SIFT: Utilizes SIFT to detect and match features, ensuring robust tracking even under varying conditions.
* Interactive Bounding Box Selection: Allows the user to select the object to track by drawing a bounding box in the first frame.
* Real-Time Processing: Processes each frame of the video to update and display the object's position.

## Feature Extraction

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/sift/features.png" title="Feature Detection" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Demo

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/sift/demo.mp4" title="Example Video" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
