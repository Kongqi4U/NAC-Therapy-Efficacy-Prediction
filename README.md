# Project: Deep Learning for Breast Cancer Neoadjuvant Chemotherapy (NAC) Efficacy Prediction

*Status: Completed (Undergraduate Thesis Project)*

## 1. Project Overview

This project, my undergraduate thesis, focuses on predicting the efficacy of Neoadjuvant Chemotherapy (NAC) for breast cancer patients using deep learning models on ultrasound images. The primary challenge was the inherent ambiguity and fuzzy edges of tumors in ultrasound scans.

The key outcome was the development of a novel segmentation network, **MAFM-AttU_Net**, which significantly outperformed the baseline model in accurately segmenting tumor regions.

## 2. Key Achievements & Contributions

#### 🔹 Model Design and Optimization: MAFM-AttU_Net
* **Problem**: The baseline model, **AttU_Net**, struggled with the blurry boundaries of tumors in ultrasound images.
* **Solution**: I independently designed and implemented the **MAFM-AttU_Net**, which incorporates a **Multi-scale Awareness Fusion Module (MAFM)**. This module allows the network to capture features at different scales, improving its ability to identify faint tumor edges.
* **Result**: The Dice coefficient, a key metric for image segmentation accuracy, was improved from **69.5%** (baseline AttU_Net) to **73.07%**.

#### 🔹 Systematic Model Evaluation Framework
* **Responsibility**: I led the construction of a complete framework for predicting pathological complete response (pCR).
* **Methodology**: Systematically compared the performance of **3 different feature extractors** and **4 different classifiers** across various data modalities.
* **Scope**: Executed over **36 sets of comparative experiments** to validate the robustness and effectiveness of the proposed model.

#### 🔹 Data Engineering and Preprocessing
* **Dataset**: Independently constructed and preprocessed a clinical dataset of **143 patients**.
* **Pipeline**: The workflow included crucial steps such as:
    * Artifact removal from raw ultrasound images.
    * Cropping of the scan region to focus on relevant areas.
    * AI-assisted annotation to ensure high-quality ground truth labels.

## 3. Technical Details

* **Core Technologies**: `Python`, `PyTorch`, `Scikit-learn`, `Pandas`
* **Models**:
    * **Segmentation**: `AttU_Net` (Baseline), `MAFM-AttU_Net` (Proposed)
    * **Feature Extractors**: [可以具体列出，例如 ResNet, VGG等]
    * **Classifiers**: [可以具体列出，例如 SVM, RandomForest等]

## 4. Code and Results
The repository will contain the source code for the MAFM-AttU_Net model, data preprocessing scripts, and experiment logs.

---
