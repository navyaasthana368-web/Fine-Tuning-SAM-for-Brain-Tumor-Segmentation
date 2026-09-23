# Fine-Tuning SAM for Brain Tumor Segmentation

## Project Overview

This project focuses on fine-tuning the Segment Anything Model (SAM) for brain tumor segmentation using MRI images from the BraTS 2020 dataset.

The main objective is to adapt SAM, originally designed for general image segmentation, for medical image segmentation and compare its performance with a U-Net baseline model.

## Problem Statements 

Brain tumor segmentation from MRI scans is a critical task in medical image analysis. Manual segmentation is time-consuming and requires expert knowledge. This project explores deep learning-based segmentation to assist in accurate tumor region detection.

## Dataset

- Dataset: BraTS 2020
- Image Type: MRI brain scans
- Modalities Used: FLAIR and T1CE
- Task: Brain tumor segmentation

**Note:** The dataset is not included in this repository due to its size and access restrictions.

## Models Used

- U-Net baseline model
- Segment Anything Model (SAM) ViT-B
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
- Scikit-learn
- Scikit-image
- Matplotlib
- Nibabel
- tqdm
- Segment Anything Model (SAM)

## Project Structure

```text
Fine-Tuning-SAM-for-Brain-Tumor-Segmentation/
│
├── docs/
│   └── report.pdf
│
├── notebooks/
│   ├── 01-data-preprocessing.ipynb
│   ├── 02-unet-baseline.ipynb
│   ├── 03-sam-zero-shot-ipynb.ipynb
│   └── 04-sam-finetuning.ipynb
│
├── results/
│   ├── architecture_diagram.png
│   ├── model_comparison.png
│   ├── model_performance_metrics.png
│   ├── training_logs.png
│   ├── training_vs_validation.png
│   └── zero_shot_prediction.png
│
├── .gitignore
├── README.md
└── requirements.txt

## Installation

Clone the repository:

```bash
git clone https://github.com/navyaasthana368-web/Fine-Tuning-SAM-for-Brain-Tumor-Segmentation.git
