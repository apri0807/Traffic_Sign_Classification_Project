# 🚦 Traffic Sign Classification using CNN

## 📌 Overview
This project implements a **Convolutional Neural Network (CNN)** to classify traffic signs from the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset.  
Traffic sign recognition is a crucial component of autonomous driving and advanced driver assistance systems (ADAS). The model achieves **~96% accuracy** on the test set, demonstrating strong performance in real-world scenarios.

---

## 📂 Dataset
- **Source:** GTSRB dataset (Meta, Train, Test folders with CSV metadata).
- **Classes:** 43 traffic sign categories.
- **Images:** ~50,000 images captured under diverse conditions (lighting, angles, occlusion).
- **CSV Files:**
  - `Meta.csv` → metadata about images.
  - `Train.csv` → training images and labels.
  - `Test.csv` → test images and labels.

---

## ⚙️ Preprocessing
- Images resized to **32×32 pixels**.
- Normalized pixel values to range [0,1].
- Labels converted to **one-hot encoding**.
- Train-validation split (80%-20%).

---

## 🧠 Model Architecture
Implemented using **TensorFlow/Keras**:

- **Conv2D layers** → feature extraction.  
- **MaxPooling2D** → dimensionality reduction.  
- **Flatten + Dense layers** → classification.  
- **Dropout** → regularization.  
- **Softmax output** → 43 neurons for multi-class classification.  

---
