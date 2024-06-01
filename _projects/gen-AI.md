---
layout: page
title: Criminal Face Sketcher using Generative AI
description: Developed a Criminal Face Sketch Generator using Generative AI to generate accurate facial sketches and variations for streamlining investigations and forensics. Leveraged tools such as LLMs, PyTorch, Stable Diffusion models, Hugging Face Transformers, and ONNX.
img: assets/img/12.jpg
importance: 1
category: Generative AI
related_publications: false
---

# Criminal Face Generation Platform Using Stable Diffusion

## Project Overview

### Project Idea

Traditional forensic face sketch methods can be subjective, inconsistent, and time-consuming. Our project leverages stable diffusion technology to create a more accurate, objective, and efficient tool for law enforcement to generate suspect face sketches.

### Problem Significance

Current methods rely heavily on forensic artists' skills and can be slow, leading to inaccuracies as witness memories fade. This subjectivity and delay can hinder investigations and affect public trust in law enforcement.

### Problems with Existing Solutions

AI face recognition relies on existing databases and can struggle with suspects not in the system or with altered appearances. Biometric systems have their own challenges, such as data privacy concerns and the need for comprehensive databases.

## Our Solution

![Proposed System](assets/img/Proposed_system_model.png)

Our solution uses:

- **Prompt Generator LLM:** Extracts key facial features from descriptions.
- **Stable Diffusion Model:** Converts descriptions into images with high quality and diversity.
- **Image-to-Image Refiner:** Allows fine-tuning of the generated images.

This approach provides higher quality and more diverse sketches than other methods like GANs, with easier training and fewer artifacts.

## Impact

Our tool enhances the efficiency and accuracy of criminal investigations, leading to faster suspect identification and improved public trust in law enforcement.

## Architecture

![System Architecture](assets/img/System_Architecture.png)

- Prompt Generator LLM
- Image Generator Stable Diffusion Model
- Image-to-Image Refiner

## Learn More

For detailed documentation and source code, visit our GitHub repository:

[GitHub Repository](https://github.com/YourUsername/YourRepo)


