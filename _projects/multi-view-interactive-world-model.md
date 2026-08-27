---
layout: page
title: Map-Conditioned Multi-View Interactive World Modeling
permalink: /projects/multi-view-interactive-world-model/
description: Action-conditioned multi-view first-person world modeling for highly dynamic interactive environments (ongoing).
importance: 1
category: research
---

**Ongoing collaborative research · Peking University · Advised by [Prof. Hao Tang](https://ha0tang.github.io/)**

We study how to extend a large action-conditioned video model into a coherent, interactive multi-view world model. Built on _LingBot-World_, a 14B video Diffusion Transformer, the system generates synchronized first-person viewpoints in CS:GO, where rapid camera motion, abrupt scene changes, and complex interactions make long-horizon prediction especially challenging.

## System capabilities

- **Cross-view consistency:** synchronized viewpoints remain aligned with a shared underlying world state.
- **World stability:** scene structure remains stable under rapid motion and viewpoint changes.
- **Complex interaction:** generation responds to action inputs in highly dynamic gameplay.
- **Long-horizon generation:** the model sustains coherent interactive rollouts beyond short clips.

## My contributions

- Designed a residual **Map Memory conditioning adapter** with LoRA to provide an explicit spatial reference across views.
- Built the end-to-end data and evaluation pipeline from raw gameplay recordings to synchronized multi-view clips and Map Memory conditions.
- Trained and debugged the 14B model on a **16× NVIDIA H200 GPU cluster**, diagnosing failures across the data, training, and systems stack.
- Developed evaluations for spatial grounding, cross-view consistency, world stability, and long-horizon behavior.

**Status.** This work is ongoing. A manuscript and a fuller project page with qualitative results are in preparation.
