---
layout: post
title:  "Oil Painting Digitalization"
date:   2025-03-06 14:16:56 +0800
categories: project
thumbnail: /assets/images/posts/opp_hardware.png
---
This study proposes a practical method for obtaining spatially varying bidirectional reflectance distribution function (SVBRDF) textures such as diffuse map, roughness map, normal map and specular map for oil paintings with rich impasto and varying gloss. We combined the photometric stereo algorithm with a deep learning model, which was trained based on real oil painting samples.
This research project encompasses color correction, photometry, image stitching techniques, AI, and computer graphics knowledge; as well as hardware expertise in camera control and calibration, circuit design, and embedded systems.

**This research has been published as a journal article in <font color="red">Computer Graphics Forums</font>:** <https://onlinelibrary.wiley.com/doi/10.1111/cgf.70295>

## Device overview
<img src="/assets/images/posts/opp_hardware.png" alt="profile image" class="profile-image">
The figure shows the device used to capture information from oil painting samples. The "imaging module" (B in figure) contains an industrial camera, 5 LED light sources, and rotatable linear polarizers covering the camera and light sources. The imaging module was mounted on a framework which was carried by a biaxial movement system in the horizontal plane, extending the scanning area by allowing the imaging module to be translated in two directions. Subsequently, the scanned patches were stitched by adaptively blending the overlapping regions to generate a wider field of view.
## Workflow
<img src="/assets/images/posts/opp_workflow.png" alt="profile image" class="profile-image">
After capturing the photos using the imaging module, a computational process is applied to generate texture maps such as albedo (ρ), normal vector (n), roughness (R), and specular (S) maps. These maps are used in PBR (physically-based rendering) to produce a realistic representation of oil paintings.

## Demo video of digitalized oil painting
The demo video was rendered by [Blender](https://www.blender.org/), to demonstrate the appearance of oil painting under different lighting angles and from different views.
<iframe width="740" height="400" src="https://www.youtube.com/embed/sNtdmCn6wcA?si=Bt3rx5LArObXlrhy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
