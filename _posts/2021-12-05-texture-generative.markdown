---
layout: post
title:  "AI Texture Generative System"
date:   2021-12-05 14:16:56 +0800
categories: project
thumbnail: /assets/images/posts/spgan_result.png
---
I employed **Generative Adversarial Networks (GAN)** to synthesize texture images including wood, stone, and fabric. The pyramid-like network generate low resolution texture, and upsample to 32x resolution via super resolution network. 

The input noise is designed to be 2D tensor and has arbitrary size, that make the network is able to generate any size texture, For example, small (512x512) to very large (8192x8192). 

This research project utilized **TensorFlow** to build and train both GAN and super-resolution network. The system serves the interior decoration industry by creating stylish elements for tiles and wallpaper, and can generate texture maps for application in 3D realistic rendering.


<img src="/assets/images/posts/spgan_net.png" alt="spgan_net.png" class="profile-image">
Pyramid-like network structure.

<img src="/assets/images/posts/spgan_result.png" alt="spgan_result.png" class="profile-image">
Generated result of difference method. Reference ground truth image are 512x512, result image are 1024x1024.