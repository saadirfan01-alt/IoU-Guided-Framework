# IoU-Guided Dual-Path Multi-Task Network for Polyp Detection and Segmentation

## Overview

This repository provides the implementation of the proposed IoU-guided dual-path multi-task framework for simultaneous polyp detection and segmentation in colonoscopy images.

The model combines:

* A YOLO-inspired detection branch for object localization
* A UNET-based segmentation branch for pixel-wise prediction
* A partially shared backbone for feature reuse
* An IoU-guided fusion mechanism to enforce spatial consistency between detection and segmentation

## DOI

https://doi.org/10.5281/zenodo.19511982

---

## Requirements

Install dependencies using:

pip install -r requirements.txt

---

## Dataset Setup

### Kvasir-SEG (Training and Evaluation)

Download:
https://www.kaggle.com/datasets/tanmaydebnath/kvasir-seg-dataset

Organize as:

Kvasir-SEG/
├── images/
├── masks/

---

### CVC-ClinicDB (Cross-Dataset Testing)

Download:
https://www.kaggle.com/datasets/balraj98/cvcclinicdb

Use:

CVC/
├── PNG/
├── Original/

---

## How to Run

1. Install dependencies:
   pip install -r requirements.txt

2. Open the notebook:
   Dual-Path.ipynb

3. Run all cells sequentially to:

* Train the model
* Evaluate performance
* Generate Grad-CAM visualizations

---

## Expected Results

On Kvasir-SEG:

* mIoU ≈ 93.7%
* IoU ≈ 92.7%
* AUC ≈ 0.97
* Average Precision (AP) ≈ 0.93

Cross-dataset evaluation on CVC-ClinicDB demonstrates strong generalization without fine-tuning.

---

## Features

* Dual-path detection and segmentation
* IoU-guided fusion mechanism
* Multi-task learning framework
* Grad-CAM based interpretability
* Cross-dataset evaluation

---

## Reproducibility

This repository includes:

* Full model implementation
* Training and evaluation pipeline
* Dataset preprocessing steps
* Experimental configuration

All results reported in the paper can be reproduced by following the steps above.

---

## Citation

If you use this work, please cite:

An IoU-Guided Dual-Path Multi-Task Network for Polyp Detection and Segmentation in Colonoscopy Images
The Visual Computer
