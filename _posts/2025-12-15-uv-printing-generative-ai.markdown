---
layout: post
title:  "Generative AI for UV Color Printing Reproduction of Oil Paintings"
date:   2025-12-15 00:00:00 +0800
categories: project
thumbnail: https://res.cloudinary.com/dx77thjfu/image/upload/v1784730768/workflow_gj58l7.png
---
This project applies generative AI to produce high-quality printed reproductions of oil paintings using UV color printing technology. From a single photograph of a painting, the system generates a height map and a gloss map that encode the physical characteristics of the original artwork — including paint layering variation, brushstroke texture, and gloss variation — enabling the printed reproduction to faithfully replicate these tactile and optical properties.

## Workflow

<img src="https://res.cloudinary.com/dx77thjfu/image/upload/v1784730768/workflow_gj58l7.png" alt="AI workflow for UV printing reproduction" class="profile-image">

The figure above illustrates the end-to-end pipeline: from single-image input through AI inference to UV print output.

## System Architecture

The project establishes a complete AI system covering training, deployment, and inference. The pipeline is designed so that PMI personnel can independently train new generative AI models, allowing the system to be continuously developed and applied to new artworks without external dependency.

Key components include:
- **Height map generation** — predicts surface relief from a flat image to encode brushstroke depth and paint accumulation
- **Gloss map generation** — captures spatially varying specular properties of the painting surface
- **UV printing integration** — maps the generated maps to UV inkjet printer parameters to reproduce physical texture and gloss variation on the printed substrate
