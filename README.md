# retina-disease-classifier
TensorFlow-based CNN that classifies retinal images into disease categories to support early detection.

# AI Powered Retinal Disease Detection with Deep Learning and Computer Vision Pipeline

A complete end to end computer vision pipeline for classifying retinal fundus images into four categories — **cataract, diabetic retinopathy, glaucoma, and normal** — using **TensorFlow Keras**, **EfficientNet**, and **transfer learning**.

This project demonstrates how deep learning can support early ophthalmic screening by automatically flagging at risk patients for follow up with clinicians.

---

## 🔬 Project Overview

This repository contains a deep learning based medical imaging pipeline built to:

- Ingest and preprocess high resolution retinal images  
- Train a multi class classifier using an EfficientNet backbone  
- Evaluate model performance with robust metrics  
- Provide interpretable outputs suitable for clinical screening workflows  

Dataset: **4000+ retinal fundus images (456×456 px)** labeled as **cataract**, **diabetic retinopathy**, **glaucoma**, or **normal**.

---

## 👤 Role  
**Lead ML Engineer and Computer Vision Researcher**

## 🩺 Domain  
Medical Imaging · Ophthalmology · Clinical Decision Support

## 🛠️ Tech Stack  
Python · TensorFlow Keras · EfficientNet B models  
NumPy · Pandas  
Matplotlib · Plotly  

---

## ⚡ Quick Facts
- Task: Multi class retinal disease classification  
- Approach: Transfer learning with EfficientNet CNN  
- Image Size: 456×456 px  
- Skills Demonstrated: Computer vision, augmentation, deep learning, class imbalance handling, reproducibility, pipeline design  

---

# Background and Problem Statement

Diabetic eye diseases — cataracts, diabetic retinopathy, and glaucoma — are among the leading causes of preventable blindness. Early detection through retinal imaging improves clinical outcomes, but manual review is:

- Time consuming  
- Subjective  
- Dependent on specialists who may be unavailable in many settings  

Modern CNNs achieve strong performance on medical imaging tasks, yet real clinical workflows require more than a single model. A full system must support:

- Data ingestion and preprocessing  
- Augmentation  
- Reproducible training  
- Evaluation and reporting  
- Model interpretability  

**Problem Statement:**  
*Can we design an accurate and reproducible deep learning pipeline to classify retinal images into common disease categories and normal, in a way that supports potential clinical integration?*

---

# Model Development

## 1. Dataset Preparation  
- Over 4000 retinal fundus images collected and standardized  
- Resized to 456×456 px to preserve vessels, optic disc structure, and lesion detail  
- Stratified train, validation, and test splits  

---

## 2. Preprocessing and Augmentation  
- Standard resizing and normalization  

---

## 3. Model Architecture and Training Strategy  

### Architecture
- EfficientNet backbone with pretrained ImageNet weights  
- Custom classifier head with global average pooling, dense layers, dropout, and softmax  

### Training
- Stage 1: Freeze backbone and train classification head  
- Stage 2: Unfreeze upper EfficientNet blocks and fine tune  
- Optimizer: Adam  
- Loss: Categorical cross entropy  
- Metrics: Accuracy, precision, recall, F1  

---

## 4. Model Evaluation  
Evaluation performed on a held out test set with:

- Overall accuracy  
- Per class precision, recall, and F1  
- Confusion matrix  
- Loss and accuracy learning curves  

Class imbalance handled using **class weights** and augmentation.

---

# Computer Vision Pipeline and Reproducibility

A pipeline oriented design ensures rerun ability, clarity, and future extensibility.

### End to End Pipeline Steps
- Data loading  
- Preprocessing  
- Augmentation  
- Model construction  
- Training  
- Evaluation  

### Reproducibility Practices
- Fixed seeds  
- Explicit dataset splits  
- Configurable parameters  
- Modular notebook and script based workflow  

---

# Results

The model successfully distinguishes four retinal conditions by learning fine structural and vascular cues.

Outputs include:

- Confusion matrix  
- Per class metrics  
- Learning curves  

---

# Impact and Actionable Insights

Even though this project is research oriented, it demonstrates a full stack healthcare ML workflow.

### Clinical Insight  
- Demonstrates how AI can assist clinicians by screening retinal images for potential abnormalities  

### Pipeline Reusability  
- Easily generalized to other medical imaging tasks such as chest X rays or dermoscopy  

### Model Governance Alignment  
- Clear structure from data to evaluation supports auditing and clinical validation requirements  

### Portfolio Relevance  
This project highlights skills in:

- Computer vision  
- EfficientNet and transfer learning  
- Managing class imbalance  
- Reproducible ML engineering  

These are highly relevant to modern data scientist and ML engineer roles.





