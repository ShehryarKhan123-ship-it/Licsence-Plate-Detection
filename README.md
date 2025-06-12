# 🚗 License Plate Detection and Segmentation System

[![Python](https://img.shields.io/badge/Language-Python-blue.svg?logo=python)](https://www.python.org/)
[![YOLOv11](https://img.shields.io/badge/Model-YOLOv11-success)](https://github.com/WongKinYiu/yolov7)
[![SAM](https://img.shields.io/badge/Segmenter-SAM-orange)](https://github.com/facebookresearch/segment-anything)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Made with ❤️](https://img.shields.io/badge/Made%20with-%E2%9D%A4-red)](#)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/your_notebook_link_here)

This repository contains a robust system for **License Plate Detection and Segmentation** in vehicle images. The project leverages the power of **YOLOv11** for accurate license plate detection and **SAM (Segment Anything Model)** for precise segmentation. The system has achieved an impressive **97% detection accuracy** on the test set.

---

## 📌 Features

- 🔍 **License Plate Detection** using YOLOv11 (custom-trained on annotated dataset)
- ✂️ **Segmentation** of license plates using Meta's Segment Anything Model (SAM)
- 📈 Achieved **97% model accuracy**
- 🖼️ Supports batch image processing
- 🧠 Custom training on Roboflow dataset
- 💡 Easy integration and deployment-ready

---

## 🧪 Demo

https://drive.google.com/file/d/1IM8LexXvXOE2qhcUbxvDQNnRZjMBgnU7/view?usp=sharing 

> Example of license plate detection and mask-based segmentation.

---

## 🚀 Getting Started

### 1. Clone the Repository

```python
git clone https://github.com/ShehryarKhan123-ship-it/license-plate-detection.git
cd license-plate-detection
```
### 2.Install Dependencies

```python
pip install -r requirements.txt
```
### 3.🧠 Model Details

📌 YOLOv11 Detection
Trained using Roboflow annotated license plate dataset

Achieved 97% mAP on test data

Fast and lightweight for real-time detection

📌 SAM Segmentation
Uses bounding boxes from YOLO to generate masks

Supports pixel-accurate segmentation of detected license plates


### 4 .🛠️ How to UseDetect and Segment Plates
```bash
python src/detect.py --source path/to/image.jpg --weights yolo_weights/best.pt
python src/segment.py --image path/to/detected_image.jpg --sam-model sam_model/sam_vit_h.pth
```
### 5.📦 Dependencies
-Python 3.8+

-YOLOv11

-Segment Anything (SAM)

-PyTorch

-OpenCV

-NumPy

-Matplotlib

### 6. 📁 Dataset
The model was trained on a custom-labeled dataset from Roboflow.
You can import the dataset using Roboflow's Python SDK or download it manually.

### 7. 📜 License
This project is licensed under the MIT License – see the LICENSE file for details.
