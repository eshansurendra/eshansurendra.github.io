---
layout: page
title: Handwritten Digit Classifier
description: The Handwritten Digit Classifier is a machine learning project that utilizes TensorFlow to classify handwritten digit images from the MNIST dataset. This project demonstrates the complete workflow of image classification, from data preprocessing to model evaluation and visualization.
img: assets/img/handwritten/handwritten_thumb.jpg
importance: 3
category: software
tags : ['Tensorflow', 'keras', 'MNIST', 'Machine learning']
related_publications: false
github: https://github.com/eshansurendra/handwritten-digit-classification
---

> For detailed documentation and source code, visit our [GitHub Repository](https://github.com/eshansurendra/handwritten-digit-classification).

## Overview

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/handwritten/overview.png" title="overview" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Dataset

The project uses the MNIST dataset, a standard benchmark in the field of image classification. It consists of 70,000 grayscale images of handwritten digits, split into 60,000 training images and 10,000 testing images. Each image is `28x28 pixels` in size and labeled with a digit from 0 to 9.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/handwritten/dataset.png" title="dataset" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Architecture

The neural network architecture includes an input layer with 784 neurons (one for each pixel in the 28x28 images), two hidden layers for learning complex patterns, and an output layer with 10 neurons corresponding to the digit classes (0-9). This structure enables the model to effectively capture and classify handwritten digits.

```python
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense

model = Sequential([
    Dense(128, activation='relu', input_shape=(784,)),
    Dense(128, activation='relu'),
    Dense(10, activation='softmax')
])
```
## Results

This simple model resulted in a accuracy over 97.69%. The validation accuracy was 98.5%. As shown in the image below, the model has predicted the label(digit) for most images correctly.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/handwritten/handwritten_thumb.jpg" title="handwritten_thumb" class="img-fluid rounded z-depth-1" %}
    </div>
</div>



