# FaceShield: High-Utility Differential Privacy Facial Protection for Online Image Publishing

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-brightgreen.svg)](https://creativecommons.org/licenses/by-nc/4.0/) ![PyTorch](https://img.shields.io/badge/Pytorch-2.6.0-brightgreen) ![Python](https://img.shields.io/badge/Python-3.10.16-brightgreen)

<b> Authors: Ming Zhang, Yuchen Hui, <a href='https://scholar.google.com/citations?hl=zh-CN&user=y52WOmkAAAAJ&view_op=list_works&sortby=pubdate'>Xiaoguang Li*</a>, Guojia Yu, <a href='https://scholar.google.com/citations?hl=zh-CN&user=FFX0Mj4AAAAJ'>Haonan Yan</a>, <a href='https://scholar.google.com/citations?hl=zh-CN&user=oEcRS84AAAAJ&view_op=list_works&sortby=pubdate'>Hui Li*</a>  </b>

---
## 📚 **Overview**
<div align="center"> 
</div>
<div style="text-align:center;">
  <img src="figures/framework.png" style="max-width:60%;">
</div>

Welcome to FaceShield, your high-fidelity and provable facial privacy protection platform! Here are some key features of our platform:

> 📌 **Feature disentanglement**: *FaceShield* leverages joint statistical and spatial independence constraints to maximally disentangle facial identity and perceptual content, thereby separating identity perturbation from perceptual preservation.
> 
> 📌 **Practical Sampling**: *FaceShield* decomposes high-dimensional identity perturbation into two tractable sub-processes, thereby reducing computational overhead in high-dimensional scenarios.
> 
> 📌 **Comprehensive Protection**: *FaceShield* prevents unintended identity leakage arising from the perceptual latent space, offering users comprehensive facial privacy protection.
> 
> 📌 **Extensive Evaluation**: *FaceShield* offers users a superior and reliable solution in terms of naturalness, perceptual fidelity, privacy protection, and efficiency.

---

## 😊 **FaceShield Updates**
> - [ ] To be supplemented code after acceptance...
>
> - [x] 09/11/2026: *First version pre-released for this open source code.* 
---

<font size=4><b> Table of Contents </b></font>

- [Quick Start](#-quick-start)
  - [Environmental](#1-Environmental)
  - [Download Data](#2-download-data)
  - [Preprocessing](#3-preprocessing)
  - [Training](#4-Training)
  - [Evaluation](#5-evaluation)
- [Results](#-results)
- [Citation](#-citation)
- [Copyright](#%EF%B8%8F-license)

---

## ⏳ Quick Start

This repository contains the implementation pipeline for FaceShield. It first requires environment setup via Conda and dependency installation. Next, users prepare two core datasets, FF-HQ and VGGface2, placing them in the specified directory or configuring the root path in training scripts. A preprocessing script then runs on the datasets to compute and save neuron weight information required by the model.

FaceShield adopts a two-stage training strategy. The Feature Separation Extractor (FSE) is trained first, followed by the Image Reconstructor (IRC). Users launch distributed training with designated GPU IDs and adjust training epochs. Intermediate checkpoints are automatically saved at fixed batch intervals for both stages. After training completes, evaluation can be performed using `test.py` with pre-trained weights, input images and configurable perturbation parameters.

We will release the specific details after the paper is accepted.

## 🏆 Results

<a href="#top">[Back to top]</a>

We present partial experimental results for FaceShield. For a comprehensive understanding of FaceShield's performance in terms of perceptual fidelity, facial privacy protection, and sampling efficiency, we strongly recommend referring to our [paper](xxx).

<div align="center"> 
</div>
<div style="text-align:center;">
  <img src="figures/effect.jpg" style="max-width:60%;">
</div>

These resources provide a detailed analysis of the training outcomes and offer a deeper understanding of the methodology and findings.

## 📝 Citation

<a href="#top">[Back to top]</a>

If you find our benchmark useful to your research, please cite it as follows:

```
coming soon.
```

## 🛡️ License

<a href="#top">[Back to top]</a>

If you have any suggestions, comments, or wish to contribute code or propose methods, we warmly welcome your input. Please contact us at zhangming2025@njust.edu.cn or huiyc@stu.xidian.edu.cn. We look forward to collaborating with you in pushing the boundaries of facial privacy protection.

