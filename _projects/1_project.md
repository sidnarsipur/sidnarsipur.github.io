---
layout: page
title: PBR Texture Generation
description: Generate texture maps from photographs
category: cs
img: assets/img/TextGen2.png
importance: 1
---

[Github](https://github.com/sidnarsipur/TextGen)

Materials are vital for computer graphics and are widely used across domains (animation, 3D modelling, mixed real- ity). However, their creation remains challenging, even for experts.

Physically Based Rendering (PBR) is a modern approach to shading and rendering materials. PBR materials use texture maps that encode different stylization and details such as height, metallicness etc., that are then combined and applied to the surface of 3D models to create patterns or define visual effects. Basecolor (Albedo) maps are the input that defines the color or reflectivity of the surface. While creating Albedo maps for PBR materials is straight-forward, they define just the base color and lack the complexity needed for realistic textures.

I used ControlNet, a deep learning algorithm used for controlled image generation, and trained it to generate normal and roughness texture maps, utilizing only the base color (Albedo Map) as the conditioning input. Based on testing, the models also worked well on receiving material photographs.

[Dataset](https://huggingface.co/datasets/sidnarsipur/controlnet_data)  |
[Model-1](https://huggingface.co/sidnarsipur/controlnet_normal)  | [Model-2](https://huggingface.co/sidnarsipur/controlnet_rough)  |
[Report](https://github.com/sidnarsipur/TextGen/blob/main/Report.pdf)  |

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/TextGen.png" title="Poster" class="img-fluid rounded z-depth-1" %}
  </div>
</div>



