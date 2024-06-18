---
layout: page
title: Semantic segmentation of aerial imagery using U-Net
description: Implementation of a semantic segmentation model for aerial imagery using the U-Net architecture. The project aims to accurately segment various objects and features within aerial images, leveraging the powerful capabilities of the U-Net model.
img: assets/img/aerialseg/thumb.png
importance: 4
category: software
tags : ['unet', 'sementic-segmentation', 'tensorflow']
related_publications: false
github: https://github.com/eshansurendra/AerialSeg-U-Net
---

> For detailed documentation and source code, visit this [GitHub Repository](https://github.com/eshansurendra/AerialSeg-U-Net).
> For a more comprehensive understanding of the implementation, refer this [notebook on Kaggle](https://www.kaggle.com/code/eshansurendra/semantic-segmentation-using-u-net/notebook#Semantic-segmentation-of-aerial-imagery-using-U-Net)

The model is trained to recognize and classify the following classes:

* **Building:**  #3C1098
* **Land (unpaved area):** #8429F6
* **Road:** #6EC1E4
* **Vegetation:** #FEDD3A
* **Water:** #E2A929
* **Unlabeled:** #9B9B9B

# Project Overview

This project implements a semantic segmentation model for aerial imagery using the U-Net architecture. The U-Net model is a convolutional neural network specifically designed for image segmentation tasks, achieving high accuracy in segmenting various objects and features within images. The code in this repository leverages TensorFlow to implement the U-Net model and perform segmentation on aerial imagery. 

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/aerialseg/banner.png" title="banner" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## U-Net architecture

The U-Net architecture is characterized by its unique encoder-decoder structure. The encoder progressively downsamples the input image using convolutional and pooling layers, extracting hierarchical feature maps. The decoder then upsamples these features, gradually reconstructing the segmented image.  A key feature of U-Net is the use of skip connections, which combine feature maps from the encoder with corresponding decoder layers. This allows the model to retain fine-grained spatial information from the input, improving segmentation accuracy. 

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/aerialseg/unet.png" title="unet" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

This architecture makes U-Net particularly effective for semantic segmentation tasks involving complex structures and boundaries, as seen in aerial imagery.  The U-Net architecture was originally proposed in the paper ["U-Net: Convolutional Networks for Biomedical Image Segmentation"](https://arxiv.org/pdf/1505.04597) by Olaf Ronneberger, Philipp Fischer, and Thomas Brox. 

## Dataset

This project utilizes the ["Semantic segmentation of aerial imagery dataset"](https://www.kaggle.com/datasets/humansintheloop/semantic-segmentation-of-aerial-imagery), hosted on `Kaggle`. This Public Domain dataset consists of aerial imagery of Dubai, UAE, captured by MBRSC satellites and annotated with pixel-wise semantic segmentation into 6 classes. The total volume of the dataset is 72 images grouped into 6 larger tiles.

# Project Structure

**`Complete Notebook hosted on Kaggle:` [https://www.kaggle.com/code/eshansurendra/semantic-segmentation-using-u-net](https://www.kaggle.com/code/eshansurendra/semantic-segmentation-using-u-net)**

This notebook provides a comprehensive implementation of the semantic segmentation project using the U-Net model, covering data preprocessing, model building, training, and prediction steps. 

# Results

The U-Net model, trained on the "Semantic segmentation of aerial imagery" dataset, achieved promising results on the segmentation task.  This section presents the key performance metrics and visualizations to illustrate the model's capabilities. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/aerialseg/leftgraph.png" title="left image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/aerialseg/rightgraph.png" title="right image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Performance Metrics:**

* **Test Accuracy:** 87%
* **Test Jaccard Coefficient (IoU):** 0.7308
* **Test Loss:** 0.8974
* **Validation Accuracy:** 84%
* **Validation Jaccard Coefficient (IoU):** 0.6869
* **Validation Loss:** 0.9149

These metrics indicate that the model demonstrates strong generalization ability, as it performs well on both the training and validation sets.  The high accuracy and IoU scores suggest that the model effectively learns to segment aerial images into distinct object categories.

**Visualization of Segmentation Results:**

Here are examples of segmentation predictions made by the model on test images:

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/aerialseg/ex1.png" title="ex1.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/aerialseg/ex2.png" title="ex2.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/aerialseg/ex3.png" title="ex3.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
