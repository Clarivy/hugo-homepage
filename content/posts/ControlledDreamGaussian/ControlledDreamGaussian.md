---
title: "Enhancing 3D Character Generation with ControlNet and LoRA"
url: "/ControlledDreamGaussian"
date: 2023-12-28T14:47:05+08:00
draft: false
---

<div>
    <div style="display:flex;width:140px;justify-content: space-evenly;">
        <a href="/posts/ControlledDreamGaussian/images/paper.pdf">[Paper]</a>|<a href="https://github.com/KevinXu02/ControlledDreamGaussian">[Code]</a>
    </div>
</div>

![Pipeline Diagram](/posts/ControlledDreamGaussian/images/pipeline.jpg)

*Fig 1: Two-Stage Training Methodology*

## Introduction

The field of digital 3D content creation, crucial in gaming, advertising, and the emerging MetaVerse, requires efficient and sophisticated tools for generating 3D characters. This blog post delves into an innovative approach that integrates ControlNet and Low-Rank Adaptation (LoRA) into existing text-to-image diffusion models, offering a solution to common issues like spatial inconsistency and multi-view artifacts in multi-view image synthesis.

## Gallery

### 3D Model Examples

| <img src="/posts/ControlledDreamGaussian/images/hi_render.gif" width="150px"> | <img src="/posts/ControlledDreamGaussian/images/openhigh_render.gif" width="150px"> | <img src="/posts/ControlledDreamGaussian/images/openlow_render.gif" width="150px"> |
|-|-|-|

### Pose Reference Images

|Ref Image|Openpose|Generated 3D Model|
|:-:|:-:|:-:|
| <img src="/posts/ControlledDreamGaussian/images/realimage.jpg" width="150px"/> | <img src="/posts/ControlledDreamGaussian/images/keypoints1005.png" width="150px"/> | <img src="/posts/ControlledDreamGaussian/images/fight.gif" width="150px"/> |


### Training Process

<img src="/posts/ControlledDreamGaussian/images/ironman_training.gif" width="200px"/>

## Methodology

### Pipeline Overview

The methodology comprises three core components:

1. **Stable Diffusion Fine-Tuned with LoRA**: Uses Stable Diffusion for detailed image generation from text inputs. LoRA fine-tunes this model for character-specific features.

![2D Image Gallery](/posts/ControlledDreamGaussian/images/gallery.jpg)
*Samples from Fine-Tuned Stable Diffusion*

2. **ControlNet for Multi-View Consistency**: Ensures consistent character appearance from various angles using 3D body pose estimation and rendering 2D poses in random viewpoints.


3. **Generative Gaussian Splatting**: Transforms multi-view images into a cohesive 3D model, synthesizing spatial relations and depth cues.

### 3D Representations

3D information is represented through a set of 3D Gaussians. These are defined by parameters like center, scaling factor, rotation quaternion, opacity, and color.

### Text-to-3D Generation

The core process involves Score Distillation Sampling (SDS), optimizing 3D Gaussians against various camera poses and rendering RGB and transparency views.

### Noise-Free Score Distillation (NFSD)

NFSD isolates distortion-related components from predicted noise in the diffusion process, enhancing the optimization efficiency.

## Results and Analysis

### 3D Generation Process

The 3D generation process is illustrated through various training steps, highlighting the progressive development of the model.

![3D Generation Process](/posts/ControlledDreamGaussian/images/generation_process_3.png)

*Fig 3: 3D Generation Process at Different Steps*

## Challenges and Future Directions

While the approach shows promising results, challenges like lengthy generation times and the need for high-quality training sets were encountered. Future directions include leveraging CUDA programming for faster depth map generation and experimenting with multiple viewpoints rendering.
