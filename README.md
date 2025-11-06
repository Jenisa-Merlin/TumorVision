# TumorVision
Computer Vision Project - Patch to Graph Embedding Framework for Brain Tumor Classification

---

## Problem Statement

To develop a **hybrid deep learning framework** that leverages **Graph Neural Networks (GNNs)** for effective **brain tumor detection and classification** from MRI images by capturing both **spatial** and **structural** relationships among brain regions.

---

## Objectives

* Integrate **CNN-based feature extraction** with **Graph Neural Network (GNN)** modeling.
* Convert **MRI image patches** into **graph representations** to capture spatial and structural dependencies among brain regions.
* Develop a **robust, interpretable, and high-accuracy** brain tumor detection and classification model across diverse MRI scans.

---

## Tools and Technologies

* **Python**
* **Google Colab**
* **PyTorch**
* **OpenCV**
* **Matplotlib**
* **Streamlit**

---

## Dataset

**Dataset Name:** Brain MRI Images for Brain Tumor Detection
**Source:** [Kaggle Dataset Link](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection/data)

* 98 (82 unique) images **without tumor**
* 155 (140 unique) images **with tumor**

> **Note:**
> Download the dataset folders named **`yes`** and **`no`** from the above Kaggle link.
> Place them inside the folder **`brain_tumor_dataset/`** in your project directory as shown below:

```
TUMORVISION/
│
├── brain_tumor_dataset/
│   ├── yes/
│   └── no/
```
---

## Pipeline Overview

1. **Data Acquisition and Preprocessing**

   * Load and resize MRI images
   * Normalize pixel values

2. **Data Augmentation**

   * Apply rotation, flipping, and scaling to increase dataset diversity

3. **Patch Generation Module**

   * Divide MRI images into smaller patches to capture local information

4. **CNN-based Feature Extraction Module**

   * Extract spatial features from patches using a CNN backbone

5. **Graph Construction and Embedding Module**

   * Represent each patch as a node
   * Build adjacency matrix based on spatial proximity
   * Generate graph embeddings

6. **Graph Neural Network (GNN) Classification Module**

   * Classify the graph representations into **Tumor / Non-Tumor** categories

7. **Evaluation and Visualization Module**

   * Evaluate model performance using accuracy, precision, recall, F1-score
   * Visualize results using Matplotlib and Streamlit

---

## Contributors

**Team Members:** Jenisa Merlin D, Harithra R


