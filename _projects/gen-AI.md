---
layout: page
title: Criminal Face Generation Platform Using Stable Diffusion
description: Developed a Criminal Face Sketch Generator using Generative AI to generate accurate facial sketches and variations for streamlining investigations and forensics. Leveraged tools such as LLMs, PyTorch, Stable Diffusion models, Hugging Face Transformers, and ONNX.
img: assets/img/genai/gen_ai_thumb.jpg
importance: 1
category: software
tags : ['generative-AI', 'pytorch', 'stable-difusion', 'llm']
related_publications: false
github: https://github.com/eshansurendra/stable-diffusion-forensic-identification-working
---

> This project is developed for the IEEE IES Generative AI Challenge- 2024 by Team Decoders.
> For detailed documentation and source code, visit our [GitHub Repository](https://github.com/eshansurendra/stable-diffusion-forensic-identification-working).

### Project Idea

Traditional forensic face sketch methods can be subjective, inconsistent, and time-consuming. Our project leverages stable diffusion technology to create a more accurate, objective, and efficient tool for law enforcement to generate suspect face sketches.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/genai/top.jpg" title="Top Image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


### Problem Significance

Current methods rely heavily on forensic artists' skills and can be slow, leading to inaccuracies as witness memories fade. This subjectivity and delay can hinder investigations and affect public trust in law enforcement.

### Problems with Existing Solutions

AI face recognition relies on existing databases and can struggle with suspects not in the system or with altered appearances. Biometric systems have their own challenges, such as data privacy concerns and the need for comprehensive databases.

## Our Solution

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/genai/Proposed_system_model.png" title="Proposed System" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/genai/Proposed_system_model.png" title="Proposed System" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Our solution uses:

- **Prompt Generator LLM:** Extracts key facial features from descriptions.
- **Stable Diffusion Model:** Converts descriptions into images with high quality and diversity.
- **Image-to-Image Refiner:** Allows fine-tuning of the generated images.

This approach provides higher quality and more diverse sketches than other methods like GANs, with easier training and fewer artifacts.

## Impact

Our tool enhances the efficiency and accuracy of criminal investigations, leading to faster suspect identification and improved public trust in law enforcement.

## Architecture

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/genai/System_Architecture.png" title="System Architecture" class="img-fluid rounded z-depth-1" %}
    </div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/genai/System_Architecture.png" title="System Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
</div>

- Prompt Generator LLM
- Image Generator Stable Diffusion Model
- Image-to-Image Refiner

