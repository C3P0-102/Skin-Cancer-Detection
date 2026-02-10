# Skin Cancer Detection using CNN & OpenCV

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Keras](https://img.shields.io/badge/Keras-2.0%20+-red)
![OpenCV](https://img.shields.io/badge/OpenCV-4.0%20+-green)
![Kaggle](https://img.shields.io/badge/Data-Kaggle-lightblue)

## 📋 Overview
This project develops an automated image classification pipeline to assist in the identification of skin cancer. By utilizing a **Convolutional Neural Network (CNN)**, the system analyzes dermatoscopic images of moles to extract visual features—such as border irregularity and color variegation—indicative of potential malignancy.



---

## 🛠 Tools & Technologies

### **Development & Execution**
* **VS Code:** Primary IDE for local script development, modular coding, and version control.
* **Google Colab:** Utilized for high-performance model training using cloud-based GPU acceleration.

### **Core Frameworks**
* **Python:** The core programming language.
* **Keras (TensorFlow):** Used to design, compile, and train the deep learning CNN models.
* **OpenCV:** The backbone for image preprocessing, handling everything from noise reduction to data augmentation.

### **Data Source**
* **Kaggle:** The model utilizes high-quality datasets (such as HAM10000 or ISIC) sourced from Kaggle to ensure a diverse range of skin lesion samples for training.

---

## ⚙️ Pipeline Workflow

### 1. Image Preprocessing (OpenCV)
Before training, raw images are processed to improve feature clarity:
* **Resize & Crop:** Normalizing images to a consistent input size (e.g., $128 \times 128$ or $224 \times 224$).
* **Normalization:** Scaling pixel values to a range of $[0, 1]$ for faster gradient convergence.
* **Noise Reduction:** Applying Gaussian filters to remove artifacts that could mislead the model.

### 2. Feature Extraction (CNN)
The integrated neural network analyzes the moles through:
* **Convolutional Layers:** Detecting low-level patterns (edges) and high-level features (asymmetry, texture).
* **Pooling Layers:** Reducing spatial dimensions to focus on the most critical visual data.
* **Dense Layers:** Mapping extracted features to specific diagnostic categories.



---

## 🚀 Getting Started

### Prerequisites
* Python 3.x
* Kaggle API Key (to download datasets)

### Installation
1.  **Clone the repo:**
    ```bash
    git clone [https://github.com/yourusername/skin-cancer-cnn.git](https://github.com/yourusername/skin-cancer-cnn.git)
    cd skin-cancer-cnn
    ```
2.  **Install requirements:**
    ```bash
    pip install tensorflow opencv-python matplotlib pandas numpy
    ```

---

## 📚 References
* **Keras Documentation:** [Official Site](https://keras.io/)
* **OpenCV Tutorials:** [Official Site](https://docs.opencv.org/)
* **Kaggle Dataset:** [Skin Cancer MNIST: HAM10000](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000)

---

## ⚠️ Medical Disclaimer
This software is a **prototype** for educational and research purposes. It is not a medical device and should not be used for self-diagnosis. Always consult a licensed dermatologist for medical concerns.
