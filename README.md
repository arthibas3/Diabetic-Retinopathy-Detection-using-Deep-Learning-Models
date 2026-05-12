# 👁️ Diabetic Retinopathy Detection System

An AI-powered Deep Learning system for detecting and classifying **Diabetic Retinopathy** from retinal fundus images using CNNs, Transfer Learning, and Hybrid Deep Learning architectures.

---

## 🖥️ Tech Stack
- **Programming Language**: Python
- **Deep Learning Framework**: TensorFlow / Keras
- **Computer Vision**: OpenCV
- **Data Processing**: NumPy, Pandas
- **Visualization**: Matplotlib, Seaborn
- **Model Explainability**: Grad-CAM
- **Development Environment**: Jupyter Notebook

---

## 🚀 Quick Start

### Prerequisites
- Python ≥ 3.9
- Jupyter Notebook
- pip package manager

---

## 📦 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/diabetic-retinopathy-detection.git
cd diabetic-retinopathy-detection
```

### 2. Install Dependencies
```bash
pip install tensorflow opencv-python matplotlib seaborn scikit-learn numpy pandas
```

### 3. Launch Jupyter Notebook
```bash
jupyter notebook
```

Open:
```bash
Soft.ipynb
```
OR
```bash
final (2).ipynb
```

---

## 📁 Project Structure

```bash
Diabetic-Retinopathy-Detection/
│
├── Soft.ipynb                  # Baseline CNN + VGG16 implementation
├── final (2).ipynb             # Hybrid CNN + MobileNet implementation
├── baseline_cnn_dr.keras       # Saved trained model
├── dataset/
│   └── retinal_images/         # Retinal fundus image dataset
│
└── README.md
```

---

## 📊 Dataset

The project uses retinal fundus images for multi-class classification of Diabetic Retinopathy severity levels.

### Classification Categories
- No DR
- Mild DR
- Moderate DR
- Severe DR
- Proliferative DR

### Data Processing Techniques
- Image Rescaling
- Rotation Augmentation
- Zoom Augmentation
- Horizontal & Vertical Flipping
- Validation Splitting

Dataset loading and augmentation are handled using TensorFlow's `ImageDataGenerator`.

---

## 🧠 Model Architectures

### 1️⃣ Baseline CNN Model
A custom Convolutional Neural Network built using:
- Convolution Layers
- MaxPooling Layers
- Dense Layers
- Dropout Regularization
- Softmax Classification

Purpose:
- Establish baseline performance
- Compare against advanced architectures

---

### 2️⃣ VGG16 Transfer Learning Model
Implemented using pretrained **VGG16** weights from ImageNet.

### Features
- Pretrained feature extraction
- Frozen convolution base
- Custom classification head
- Improved feature learning
- Better accuracy than baseline CNN

---

### 3️⃣ Hybrid CNN + MobileNet Model
A hybrid architecture combining:
- Custom CNN branch
- MobileNet transfer learning branch

Both extracted feature maps are concatenated before final classification.

### Advantages
- Improved feature extraction
- Lightweight architecture
- Better generalization
- Reduced overfitting
- Higher prediction performance

---

## ⚙️ Training Process

### Optimizer
```python
Adam Optimizer
```

### Loss Function
```python
Categorical Crossentropy
```

### Techniques Used
- Early Stopping
- Fine-Tuning
- Validation Monitoring
- Data Augmentation

---

## 📈 Evaluation Metrics

The models are evaluated using:

- Training Accuracy
- Validation Accuracy
- Loss Curves
- Classification Performance
- Validation Loss

Graphs are visualized using Matplotlib.

---

## 🔥 Grad-CAM Visualization

The project implements **Grad-CAM (Gradient-weighted Class Activation Mapping)** to visualize which regions of retinal images influence predictions.

### Benefits
- Model Explainability
- Medical Transparency
- Better Clinical Interpretation
- Visual Attention Mapping

---

## 🔍 Workflow

```text
Retinal Image Input
        ↓
Preprocessing & Augmentation
        ↓
CNN / VGG16 / Hybrid Model
        ↓
Model Training
        ↓
Prediction & Classification
        ↓
Grad-CAM Visualization
        ↓
Performance Evaluation
```

---

## 🎯 Features

- Retinal image classification
- Baseline CNN implementation
- Transfer Learning with VGG16
- Hybrid CNN + MobileNet architecture
- Image preprocessing and augmentation
- Training and validation visualization
- Grad-CAM explainability
- Model saving and evaluation
- Deep learning-based medical image analysis

---

## 📌 Applications

- AI-assisted diabetic screening
- Ophthalmology support systems
- Healthcare automation
- Medical image analysis
- Early disease detection systems

---

## 🔧 Future Enhancements

- Deploy as a web application
- Add real-time prediction support
- Integrate cloud deployment
- Improve dataset balancing
- Add additional transfer learning models
- Generate automated medical reports
- Build a clinical decision support system

---

## 📊 Results

The Hybrid CNN + MobileNet model achieved improved classification performance compared to the baseline CNN model through:

- Transfer Learning
- Fine-Tuning
- Advanced Feature Extraction
- Data Augmentation
- Hybrid Architecture Integration

---

## 🏁 Conclusion

This project demonstrates the application of Deep Learning and Transfer Learning techniques for accurate detection of Diabetic Retinopathy from retinal fundus images. The hybrid architecture enhances prediction performance, while Grad-CAM improves interpretability for healthcare applications.

---

