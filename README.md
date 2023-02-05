<h1 align="center">
  <br>
BIGRoC: Boosting Image Generation via a Robust Classifier
  <br>
</h1>
<p align="center">
  <a>Roy Ganz</a> •
  <a>Michael Elad</a>
</p>

<p align="center">
  <img src="https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/bigroc-boosting-image-generation-via-a-robust/image-generation-on-imagenet-128x128">
  <img src="https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/bigroc-boosting-image-generation-via-a-robust/image-generation-on-imagenet-256x256">
</p>

<h4 align="center">This repository contains code for the paper "BIGRoC: Boosting Image Generation via a Robust Classifier"</h4>


<p align="center">
  <img src="https://github.com/royg27/BIGRoC/blob/main/assets/teaser_adversarial_boost.png" height="120">
</p>

# BIGRoC

> **BIGRoC: Boosting Image Generation via a Robust Classifier**<br>
> Roy Ganz, Michael Elad<br>
>
> **Abstract:** *The interest of the machine learning community in image synthesis has grown significantly in recent years, with the introduction of a wide range of deep generative models and means for training them.
In this work, we propose a general model-agnostic technique for improving the image quality and the distribution fidelity of generated images, obtained by any generative model.
Our method, termed BIGRoC (Boosting Image Generation via a Robust Classifier), is based on a post-processing procedure via the guidance of a given robust classifier and without a need for additional training of the generative model.
Given a synthesized image, we propose to update it through projected gradient steps over the robust classifier, in an attempt to refine its recognition.
We demonstrate this post-processing algorithm on various image synthesis methods and show a significant improvement of the generated images, both quantitatively and qualitatively, on CIFAR-10 and ImageNet.
Specifically, BIGRoC improves the image synthesis state of the art on ImageNet 128x128 by 14.81%, attaining an FID score of 2.53 and on 256x256 by 7.87%, achieving an FID of 3.63.*

## Citation

Ganz, Roy, and Michael Elad. "BIGRoC: Boosting Image Generation via a Robust Classifier." Transactions on Machine Learning Research (2023).

>
    @article{
    ganz2022bigroc,
    title={{BIGR}oC: Boosting Image Generation via a Robust Classifier},
    author={Roy Ganz and Michael Elad},
    journal={Transactions on Machine Learning Research},
    issn={2835-8856},
    year={2022},
    url={https://openreview.net/forum?id=y7RGNXhGSR},
    note={}
    }


<h4 align="center">Preprint on ArXiv: <a href="https://arxiv.org/abs/2108.03702">2108.03702</a></h4>
    
## Prerequisites

The entire code is contained in Colab jupiter notebook to facilitate the environment installation. Each such notebook is self-contained with the relevant package installation and explanations.

## Repository Organization

|File name         | Content |
|----------------------|------|
|`/CIFAR10`| Notebooks for Section 5.1 - experimenting BIGRoC on CIFAR-10 image generators, both conditional and unconditional|
|`/ImageNet`| Notebooks for Section 5.2 - experimenting BIGRoC on ImageNet 128x128 & 256x256 image generators, both conditional and unconditional|
|`/Comparison`| Notebooks for Section 5.3 - experimenting BIGRoC on CIFAR-10 and ImageNet using SN-ResNetGAN|


## Credits
* Robustness Package - [Code](https://github.com/MadryLab/robustness).
* FID is calculated natively in PyTorch using Seitzer implementation - [Code](https://github.com/mseitzer/pytorch-fid)
* Mimicry - [Code](https://github.com/kwotsin/mimicry), [Paper](https://arxiv.org/abs/2005.02494)
* Guided-Diffusion - [Code](https://github.com/openai/guided-diffusion), [Paper](https://arxiv.org/abs/2105.05233)


