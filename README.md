# IoU-Guided Dual-Path Multi-Task Network for Polyp Detection and Segmentation

## Overview

This repository contains the implementation of the IoU-guided dual-path multi-task framework for simultaneous polyp detection and segmentation in colonoscopy images.

The model integrates a YOLO-inspired detection branch with a UNET-based segmentation branch using a partially shared backbone and IoU-guided fusion.

## DOI

https://doi.org/10.5281/zenodo.19511982

## Requirements

Install dependencies using:

pip install -r requirements.txt

## Dataset

### Kvasir-SEG (Training)

Download from:
https://www.kaggle.com/datasets/tanmaydebnath/kvasir-seg-dataset

Place:

* images → /Kvasir-SEG/images
* masks → /Kvasir-SEG/masks

### CVC-ClinicDB (Testing)

Download from:
https://www.kaggle.com/datasets/balraj98/cvcclinicdb

Use:

* PNG/Original folder

## How to Run

Open the notebook:

main.ipynb

Run all cells sequentially.

## Features

* Dual-path detection + segmentation
* IoU-guided fusion
* Multi-task learning
* Grad-CAM visualization
* Cross-dataset evaluation

## Citation

If you use this work, please cite:

"An IoU-Guided Dual-Path Multi-Task Network for Polyp Detection and Segmentation in Colonoscopy Images"
The Visual Computer

