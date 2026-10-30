# RecLoop

**Recurrent State Modeling for Looped Transformers**

Cheng Liang¹, Tengfei Zhang², Jianyu Wu¹, Wenjie DU³, Changlian Ma⁴, Ya Zhang¹, Yanfeng Wang¹,*

¹ Shanghai Jiaotong University · ² University of Science and Technology of China · ³ Nanyang Technological University · ⁴ Nanjing University

\* Corresponding author: Yanfeng Wang.

RecLoop separates persistent cross-loop memory from the working state of a looped Transformer. A shared residualized GRU accumulates token-aligned history, and Dual-QKV Fusion exposes that history to attention queries, keys, and values.

- [Read the paper](assets/paper/recloop.pdf)
- [Project page source](index.html)
- [Reported results](assets/results.json)

The paper PDF includes supplementary experiments. The project page is a buildless static website suitable for GitHub Pages; no package installation is required.

Experiments cover model scales from 71M to 1.06B parameters and loop counts from 3 to 12 under a 10B-token FineWeb-Edu training budget. Scaling-law fits indicate approximately 11% fewer parameters at matched validation loss. See the paper for the evaluation protocol and limitations.

This repository contains the paper and project website. Training implementation is not included.
