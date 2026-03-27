# 🚀 NeuroSAR: Advanced AI for SAR Image Segmentation & Change Detection

## 📌 Overview
NeuroSAR is a research-grade deep learning framework for Synthetic Aperture Radar (SAR) image understanding. It focuses on semantic segmentation, change detection, and autonomous decision support for surveillance systems.

The project integrates advanced architectures, hybrid loss functions, and strong augmentation techniques to perform robustly under noisy SAR conditions (day/night, multi-polarization).

---

## 🧠 Key Features

### 🔍 Model Architecture
- ResNet-50 pretrained encoder (timm)
- Attention Gates
- Squeeze-and-Excitation (SE) blocks
- Atrous Spatial Pyramid Pooling (ASPP)
- Deep Supervision
- Exponential Moving Average (EMA)

---

### 📊 Training Enhancements
- OneCycleLR scheduler
- Mixed Precision Training (FP16)
- Differential Learning Rates
- Gradient Clipping

---

### 🧪 Loss Functions
- Focal Loss
- Lovász-Softmax Loss
- Dice Loss
- Hybrid combined loss for optimal performance

---

### 🧬 Data Augmentation
- Flip, rotation, elastic transforms
- Grid distortion
- Brightness/contrast adjustments
- Coarse dropout
- MixUp
- CutMix

---

### 📈 Metrics

#### Segmentation:
- mIoU (Mean Intersection over Union)
- F1-score
- Precision / Recall
- Pixel Accuracy

#### Change Detection:
- IoU
- F1-score
- False Alarm Rate (FAR)
- Missed Alarm Rate (MAR)


---


## 📦 Dataset
Segmentation Format

data/
 ├── train/
 │    ├── images/
 │    ├── masks/
 ├── val/
 ├── test/

Change Detection Format
data/
 ├── train/
 │    ├── before/
 │    ├── after/
 │    ├── change_masks/
 
---

## 🏋️ Training

model = NeuroSAR_UNet(...)
train_loader, val_loader, test_loader = get_loaders(...)
Adjust:
Batch size
Learning rate
Epochs
EMA decay
Augmentation parameters

---

## 📊 Results
High mIoU and F1-score
Robust to SAR noise and distortions
Strong generalization via augmentation and EMA

---

##🛰️ Applications
Military surveillance systems
Disaster monitoring
Urban change detection
Environmental monitoring
Autonomous UAV navigation

---
##👨‍💻 Author

Rishi Galla
M.Tech Robotics | ML & AI Engineer
