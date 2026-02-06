



# 🔬 Semiconductor Wafer Defect Classification & Analysis
*Revolutionizing Semiconductor Testing with AI*

![Industry](https://img.shields.io/badge/Industry-Semiconductor-blue)
![Tech](https://img.shields.io/badge/Tech-Deep%20Learning-orange)
![Python](https://img.shields.io/badge/Framework-TensorFlow%20%2F%20Keras-red)

## 🔧🌟 Project Overview
In semiconductor manufacturing, identifying defects on silicon wafers is critical for maintaining high yield and reducing costs. This repository contains a comprehensive suite of tools and research-driven notebooks designed to **automate the detection and classification of wafer map patterns** using advanced image processing and Deep Learning.
!![SEMICONDUCTOR WAFER](c3b040ba-d7ce-4fd5-b647-c7beaa6beecc.png)
---

## 🚀 Core Research & Workflows

### 📂 Main Analysis: `Semiconductor_Wafer_Defect_Classification.ipynb`
This is the primary implementation notebook. It covers the end-to-end pipeline:
* **Data Augmentation:** Balancing the highly skewed classes of wafer defects.
* **Feature Extraction:** Using spatial filtering to highlight defect clusters.
* **Neural Architecture:** A custom CNN designed to recognize patterns like *Donut, Scratch, Edge-Loc, and Near-full*.

### 📂 Paper Implementations: `ResearchPaper1.ipynb` & `rp2_0.ipynb`
These notebooks focus on reproducing state-of-the-art results from semiconductor manufacturing literature, specifically focusing on:
* **WM-811K Dataset handling.**
* **Comparison of ResNet vs. Custom CNN architectures.**
* **Performance metrics** (Precision-Recall) essential for high-stakes manufacturing.

---

## 📊 Defect Visualization & Analysis

### **1. Wafer Map Pattern Identification**
We process raw sensor data into visual wafer maps. Below is the visualization of the common defect categories identified by the model:

![Wafer Map Patterns](5dbd5179-ac02-41d3-9a98-b83296ff2b5b.png)
*Figure 1: Examples of Center, Donut, Edge-Loc, and Random defect patterns.*

### **2. Feature Transformation**
Before feeding data into the CNN, we apply denoising and spatial transformations to ensure the model focuses on relevant defect geometry rather than background noise.

![Spatial Filtering](3a24f627-2caa-4d22-8943-e5ff544565e3.png)
*Figure 2: Raw Wafer Data vs. Denoised Spatial Features.*

---

## 🛠 Tech Stack
* **Deep Learning:** TensorFlow, Keras
* **Data Processing:** Scikit-Learn, Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn, OpenCV
* **Domain Context:** WM-811K Wafer Map Dataset

---

## 📖 How to Use
1. **Prepare Data:** Ensure the WM-811K dataset is available in your environment.
2. **Run Preprocessing:** Use `semiconductor_paper_works.ipynb` to clean and augment the data.
3. **Train & Evaluate:** Execute `Semiconductor_Wafer_Defect_Classification.ipynb` for the final model training and reporting.

```bash
# Example setup
pip install tensorflow opencv-python matplotlib pandas scikit-learn

