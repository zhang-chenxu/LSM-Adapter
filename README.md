<div align="center">
<h1>Urban Waterlogging Detection: A Challenging Benchmark and Large-Small Model Co-Adapter [ECCV2024]</h1>

[Suqi Song]<sup>1†</sup>,[Chenxu Zhang]<sup>1†</sup>,[Peng Zhang]<sup>1</sup>, [Pengkun Li]<sup>2</sup>, [Fenglong Song]<sup>3</sup>, [Lei Zhang]<sup>1*</sup>

[Chongqing University]<sup>1</sup>
[Huawei Technologies Co., Ltd.]<sup>2</sup>
[Huawei Noah's Ark Lab]<sup>3</sup>


## Abstract

Urban waterlogging poses a major risk to public safety and infrastructure. Conventional methods using water-level sensors need high-maintenance to hardly achieve full coverage. Recent advances employ surveillance camera imagery and deep learning for detection, yet these struggle amidst scarce data and adverse environmental conditions. In this paper, we establish a challenging Urban Waterlogging Benchmark (UW-Bench) under diverse adverse conditions to advance real-world applications. We propose a Large-Small Model co-adapter paradigm (LSM-adapter), which harnesses the substantial generic segmentation potential of large model and the specific task-directed guidance of small model. Specifically, a Triple-S Prompt Adapter module alongside a Dynamic Prompt Combiner are proposed to generate then merge multiple prompts for mask decoder adaptation. Meanwhile, a Histogram Equalization Adap-ter module is designed to infuse the image specific information for image encoder adaptation. Results and analysis show the challenge and superiority of our developed benchmark and algorithm.
## Overview

* [**Dual-SAM**] is a novel learning framework for high performance Marine Animal Segmentation (MAS). The framework inherits the ability of SAM and adaptively incorporate prior knowledge of underwater scenarios.

<p align="center">
  <img src="github_show/framework.png" alt="accuracy" width="80%">
</p>

* **Motivation of Our proposed Mehtod**

<p align="center">
  <img src="github_show/motivation.png" alt="arch" width="60%">
</p>

* **Multi-level Coupled Prompt**

<p align="center">
  <img src="github_show/MCP.png" alt="arch" width="60%">
</p>

* **Criss-Cross Connectivity Prediction**

<p align="center">
  <img src="github_show/c3p.png" alt="arch" width="60%">
</p>

* **Dilated Fusion Attention Module**

<p align="center">
  <img src="github_show/dfam.png" alt="arch" width="60%">
</p>


## Main Results

We rely on five public datasets and five evaluation metrics to thoroughly validate our model’s performance.
<p align="center">
  <img src="github_show/res1.png" alt="arch" width="60%">
</p>

<p align="center">
  <img src="github_show/res2.png" alt="arch" width="60%">
</p>



## Getting Started

</div>

### Installation

**step1:Clone the Dual_SAM repository:**

To get started, first clone the Dual_SAM repository and navigate to the project directory:

```bash
git clone https://github.com/Drchip61/Dual_SAM.git
cd Dual_SAM

```

**step2:Environment Setup:**

Dual_SAM recommends setting up a conda environment and installing dependencies via pip. Use the following commands to set up your environment:
#### Create and activate a new conda environment

```bash
conda create -n Dual_SAM
conda activate Dual_SAM
```
#### Install Dependencies.
```bash
pip install -r requirements.txt
```

#### Download pretrained model.
Please put the pretrained [SAM model](https://drive.google.com/file/d/1_oCdoEEu3mNhRfFxeWyRerOKt8OEUvcg/view?usp=share_link) in the Dual-SAM file.

### Model Training and Testing

**Training**
```bash
# Change the hyper parameter in the train_s.py 
python train_s.py
```

**Testing**
```bash
# Change the hyper parameter in the test_y.py 
python test_y.py
```

### Analysis Tools


```bash
# First threshold the prediction mask
python bimap.py
# Then evaluate the perdiction mask
python test_score.py
```

## Citation

```
@inproceedings{
anonymous2024fantastic,
title={Fantastic Animals and Where to Find Them: Segment Any Marine Animal with Dual {SAM}},
author={Pingping Zhang，Tianyu Yan， Yang Liu，Huchuan Lu},
booktitle={Conference on Computer Vision and Pattern Recognition 2024},
year={2024}
}
```
