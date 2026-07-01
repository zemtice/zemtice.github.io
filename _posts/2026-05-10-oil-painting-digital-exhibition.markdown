---
layout: post
title:  "Oil Painting Digital Exhibition"
date:   2026-05-10 14:16:56 +0800
categories: project
thumbnail: /assets/images/posts/sh_rendering_pipeline.png
---
The growing use of digital technologies in artistic presentation has highlighted the limitations of traditional 2D documentation, which cannot capture view-dependent optical characteristics essential for experiencing textured oil paintings. 

We present a novel approach for interactive virtual exhibition of impasto artworks. A spherical harmonics (SH)-based framework is proposed to encode the geometry and material of artwork surfaces, enabling efficient representation of complex physically-based rendering textures under varying illumination conditions. The simplified orthographic projection variant further improves computational efficiency, achieving 698.9 frames per second (FPS) on RTX 5090 and 30.4 FPS on Jetson Orin Nano. 

We demonstrate that SH-based image synthesis provides a cost-effective, scalable solution for photorealistic digital artwork presentation, bridging the gap between traditional art appreciation and interactive digital experiences.

**This research has been published as a journal article in <font color="red">Applied Optics</font>:** <https://opg.optica.org/ao/fulltext.cfm?uri=ao-65-14-4749>


## Pipeline 
<img src="/assets/images/posts/sh_rendering_pipeline.png" alt="profile image" class="profile-image">
The figure shows the encoding and rendering phases of our approach.

## Demo video of oil painting in different view
<iframe width="560" height="315" src="https://www.youtube.com/embed/UK7r8X3c_pc?si=3ihQSJngnfqfKV88" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<iframe width="560" height="315" src="https://www.youtube.com/embed/AXQGDgVHmOM?si=YK5186sP60haoy8f" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>