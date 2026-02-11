# Breast Cancer Image Classification Swim Scratch
This repository presents a simple implementation of breast cancer histopathology image classification using a Swin Transformer trained from scratch. The project investigates how hierarchical vision transformer architectures perform on medical imaging tasks without relying on pretrained weights.

The experimental pipeline follows an end-to-end training strategy. It includes loading image data from external storage, preprocessing and resizing, model construction, random weight initialization, supervised training, and performance evaluation. By removing transfer learning, the framework allows direct observation of the model’s intrinsic learning capability under limited medical data conditions.

The code is primarily designed for execution in Google Colab, but it can also be adapted to a local Jupyter Notebook environment by modifying directory paths and computational settings.

# 📂 Dataset

Due to repository size limitations, the datasets are stored externally and must be downloaded or mounted before running the notebook.

- BreakHis 200× dataset : 
https://drive.google.com/drive/folders/1fHrMNHqArqTD9XtANHzNlNDq41q9nxqj?usp=sharing

- BreastCancerImager dataset : https://drive.google.com/drive/folders/1hV7RVMtem8z2GUffm1_T3exBM32qE5zz?usp=sharing

After downloading, place the data in a directory such as data/ or update the file paths accordingly.

This project serves as a baseline educational implementation, enabling comparison between training from scratch and transfer learning strategies in breast cancer image classification

# 🧠 Implementation Overview

The notebook includes:

1. Data Preparation

- Loading image files from Google Drive
- Preprocessing such as resizing and normalization
- Data augmentation for better generalization

2. Model Setup

- Building a Swin Transformer architecture
- Initializing network parameters without pretrained weights
- Configuring the final classification head for binary or multiclass prediction

3. Training and Evaluation

- Training the model from scratch using supervised learning
- Monitoring training and validation loss
- Tracking accuracy across epochs
- Calculating classification performance metrics

This project is intended to be a simple and reproducible baseline implementation, supporting educational use and enabling comparison with transfer learning approaches.
