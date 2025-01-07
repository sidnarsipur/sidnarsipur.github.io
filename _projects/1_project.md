---
layout: page
title: TextGen
description: Normal/Roughness map generation, conditioned only on an input photograph.
img:
importance: 1
---

[Github](https://github.com/sidnarsipur/TextGen)

Texture maps have widespread use in video games, architecture and 3D modeling but are difficult to generate and design.

I used ControlNet, a deep learning algorithm used for controlling image generation, and trained it to generate normal and roughness texture maps, utilizing only the base color (Albedo Map) as the conditioning input. Based on testing, the models also worked well on receiving material photographs.

[Dataset](https://huggingface.co/datasets/sidnarsipur/controlnet_data)  |
[Model-1](https://huggingface.co/sidnarsipur/controlnet_normal)  | [Model-2](https://huggingface.co/sidnarsipur/controlnet_rough)  |
[Report](https://github.com/sidnarsipur/TextGen/blob/main/Report.pdf)  |



