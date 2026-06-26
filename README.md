# Fine-Tuning SAM for Brain Tumor Segmentation

## Project Overview
This project focuses on fine-tuning the Segment Anything Model (SAM) for brain tumor segmentation using MRI images from the BraTS 2020 dataset.

The main objective is to adapt SAM, originally designed for general image segmentation, for medical image segmentation and compare its performance with a U-Net baseline model.

## Problem Statement
Brain tumor segmentation from MRI scans is a critical task in medical image analysis. Manual segmentation is time-consuming and requires expert knowledge. This project explores deep learning-based segmentation to assist in accurate tumor region detection.

## Dataset
- Dataset: BraTS 2020
- Image type: MRI brain scans
- Modalities used: FLAIR and T1CE
- Task: Brain tumor segmentation

Note: The dataset is not uploaded in this repository due to size and access restrictions.

## Models Used
- U-Net baseline model
- Segment Anything Model ViT-B
- Fine-tuned SAM model

## Results
- U-Net baseline accuracy: around 81%
- SAM zero-shot Dice score: around 0.8473
- Fine-tuned SAM validation Dice:
  - Epoch 1: 0.8252
  - Epoch 2: 0.8340

## Technologies Used
- Python
- PyTorch
- NumPy
- Pandas
- OpenCV
- Matplotlib
- nibabel
- Kaggle GPU T4
- Segment Anything Model

## Project Structure
```text
Fine-Tuning-SAM-for-Brain-Tumor-Segmentation/
│
├── notebooks/
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_unet_baseline.ipynb
│   ├── 03_sam_zero_shot.ipynb
│   └── 04_sam_finetuning.ipynb
│
├── results/
│   ├── sample_prediction.png
│   └── training_logs.txt
│
├── docs/
│   └── minor_project_report.pdf
│
├── src/
├── README.md
├── requirements.txt
└── .gitignore