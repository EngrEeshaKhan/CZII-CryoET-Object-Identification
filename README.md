# CZII-CryoET-Object-Identification
This project builds machine learning models to automatically detect and classify protein complexes in cryo-electron tomography (cryoET) images, enabling scalable analysis of cellular structures and supporting advanced biological and medical research.
# 🧬 Cryo-ET Protein Object Identification

A high-performance deep-learning pipeline for identifying protein complexes in 3D cryo-electron tomography (cryoET) tomograms.  
Designed for clarity, reproducibility, and professional research use.

---

## 📘 Overview
Cryo-electron tomography generates high-resolution 3D views of cellular environments.  
These volumes contain thousands of tightly packed protein complexes that need automated identification for biological and medical research.

This project provides a complete machine-learning workflow for:
- 3D tomogram preprocessing  
- Feature extraction  
- Multi-class model training  
- Inference and predictions  
- Clean reproducible research structure  

---

## 🗂️ Table of Contents
- [Features](#-features)
- [Project Structure](#-project-structure)
- [Dataset](#-dataset)
- [Modeling Approach](#-modeling-approach)
- [Notebook](#-kaggle-notebook)
- [Usage](#-usage)
- [ModelPerformance](#-Model-Performance)
- [References](#-References)
- [License](#-License)

---

## ⚡ Features
✔️ 3D tomogram ingestion & preprocessing  
✔️ Deep-learning based multi-class identification  
✔️ Modular and extendable source code  
✔️ Kaggle-compatible training & inference  
✔️ GPU-ready workflow  
✔️ Clear, research-friendly architecture  

---

## 🗂️ Project Structure
<img width="218" height="293" alt="image" src="https://github.com/user-attachments/assets/c90d6fc8-8695-4a68-ace1-01e69f021350" />

---

## 🧬 Dataset

🔗 **CZII Cryo-ET Dataset (Kaggle)**  
https://www.kaggle.com/competitions/czii-cryo-et-object-identification/data

**Dataset Includes:**

| Component | Description |
|----------|-------------|
| Tomograms | High-resolution 3D cryo-ET volumes |
| Masks | Protein complex segmentations |
| Metadata | Tomogram & annotation info |
| Classes | 5 professionally curated protein complex categories |

---

## 🧠 Modeling Approach

### **1. Preprocessing**
- Volume normalization  
- 3D grid or patch generation  
- Noise reduction  
- Augmentation (optional)  

### **2. Architecture**
- 3D-CNN / adapted YOLO-3D style detector  
- Multi-class classifier  
- Spatial feature extraction  

### **3. Training Workflow**
- Balanced dataloading  
- Weighted loss for rare classes  
- GPU-trained models  

### **4. Evaluation Metrics**
- Accuracy  
- F1-score  
- IoU  
- Per-class recall  

---

## 🧪 Kaggle Notebook

📓 Full notebook implementation (training + inference):  
https://www.kaggle.com/code/eeshakhanzadi/object-czii-competition?scriptVersionId=219427511

Includes:

| Stage | Status |
|-------|--------|
| Data Loading | ✔️ |
| Preprocessing | ✔️ |
| Model Training | ✔️ |
| Eval Metrics | ✔️ |
| Prediction Pipeline | ✔️ |

---

## 🚀 Usage

### **1. Clone**
```bash
git clone https://github.com/YOUR_USERNAME/CryoET-Object-Identification.git
cd CryoET-Object-Identification
```

### **2. Train Model**
python src/train.py

### **3. Run Inference**
python src/inference.py --input sample_data/example_tomo.mrc
---
## 🏆 **Model-Performance**
<img width="673" height="157" alt="image" src="https://github.com/user-attachments/assets/768d4812-bcca-4333-9bfa-4a310a5d0bfe" />

## 📎 **References**

CryoET Dataset: https://www.kaggle.com/competitions/czii-cryo-et-object-identification/data

Training Notebook: https://www.kaggle.com/code/eeshakhanzadi/object-czii-competition

## 📄 **License**

Licensed under the MIT License.
---
