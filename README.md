# Wildfire Detection Using Machine Learning

## 📌 Overview

This project focuses on **automated wildfire smoke detection** using machine learning on satellite imagery. By leveraging convolutional neural networks (CNNs) and a Random Forest Classifier, we aim to improve the early detection of wildfires, mitigating their impact on the environment.

## 🚀 Features

- **Dataset:** USTC\_SmokeRS dataset (6,225 RGB images, 256x256 pixels)
- **Models Implemented:**
  - Simple CNN
  - Cross-Validation CNN
  - Random Forest Classifier (with ResNet18 as feature extractor)
- **Performance Evaluation:** Model accuracy, confusion matrices, and classification reports
- **Data Augmentation & Preprocessing:** Stratified splitting, normalization, and augmentation techniques applied to enhance dataset quality

## 🏗️ Tech Stack

- **Machine Learning Frameworks:** TensorFlow, PyTorch, Scikit-learn
- **Programming Language:** Python
- **Libraries:** NumPy, Pandas, Matplotlib, OpenCV

## 📂 Directory Structure

```
📁 wildfire-detection/
├── 📄 dataset/              # USTC_SmokeRS dataset (not included in repo)
├── 📄 models/               # Trained model files
├── 📄 notebooks/            # Jupyter notebooks for model training and evaluation
└── 📄 README.md             # Project documentation
```

###  Download Dataset

- The dataset is available at [USTC\_SmokeRS](https://complex.ustc.edu.cn/sjwwataset/list.htm).
- Ensure the dataset is placed in the `dataset/` directory.


## 🛠️ Model Performance

| Model                | Accuracy |
| -------------------- | -------- |
| Simple CNN           | 70.74%   |
| Cross-Validation CNN | 80.12%   |
| Random Forest        | 76.31%   |

## 📊 Results & Discussion

- The **Cross-Validation CNN** achieved the highest accuracy (80.12%), demonstrating its effectiveness in learning complex features.
- The **Random Forest Classifier** performed well, utilizing ResNet18 for feature extraction but struggled with visually similar classes.
- **Challenges:**
  - Distinguishing **smoke vs haze** was difficult due to similar visual features.
  - **Data augmentation** helped mitigate some classification errors.
  - Further improvements can be made by incorporating attention mechanisms and additional data.

---

🚀 **Early wildfire detection can save lives and ecosystems. Let's make an impact!** 🌍🔥

