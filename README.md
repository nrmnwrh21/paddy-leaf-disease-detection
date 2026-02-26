# 🌾 Paddy Leaf Disease Detection Using Deep Learning

## 📌 Project Overview

This project was developed as part of my academic exploration in Deep Learning and Computer Vision. The goal is to classify paddy leaf diseases using a Transfer Learning approach with MobileNetV2.

By applying deep learning techniques, this system helps automate disease detection from leaf images, which can support early agricultural intervention.

---

## 🎯 Objectives

- Apply Transfer Learning using MobileNetV2
- Perform dataset splitting (Train/Validation/Test)
- Improve generalization using data augmentation
- Evaluate model performance using multiple metrics
- Explore hyperparameter tuning for performance improvement

---

## 🧠 Model Approach

- Pretrained Model: **MobileNetV2 (ImageNet weights)**
- Custom Layers:
  - GlobalAveragePooling2D
  - Dense (ReLU)
  - Dropout
  - Softmax Output Layer
- Optimizer: Adam
- Loss Function: Categorical Crossentropy

The base model was frozen during initial training to utilize pretrained feature extraction.

---

## 📊 Model Performance

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

Test accuracy achieved approximately **~98–99%**, depending on tuning configuration.

---

## 🔬 Hyperparameter Tuning

I experimented with:

- Dropout rate (0.2 – 0.5)
- Dense layer units (64 – 256)
- EarlyStopping to prevent overfitting

Keras Tuner was used to compare configurations and select the best-performing model.

---

## 🏗 Project Structure

```
paddy-leaf-disease-detection/
│
├── data/
│   ├── train/
│   ├── validation/
│   └── test/
│
├── models/
│   ├── paddy_leaf_model.h5
│   ├── paddy_leaf_best_model.h5
│   └── class_labels.pkl
│
├── results/
│   ├── confusion_matrix.png
│   └── test_metrics.png
│
├── src/
│   ├── train.py
│   ├── evaluate.py
│   ├── predict.py
│   └── tune.py
│
└── requirements.txt
```

---

## 🚀 How to Run

### 1️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 2️⃣ Train Model

```bash
python src/train.py
```

### 3️⃣ Evaluate Model

```bash
python src/evaluate.py
```

### 4️⃣ Predict Image

```bash
python src/predict.py --image sample.jpg
```

---

## 📚 Learning Outcomes

Through this project, I gained hands-on experience in:

- Transfer Learning
- Image Preprocessing & Augmentation
- Model Evaluation & Metrics Interpretation
- Overfitting Prevention Techniques
- Hyperparameter Tuning
- Organizing ML Projects into Modular Structure

---

## 👩‍💻 About Me

Nur Munawwarah Binti Muzamil  
Bachelor of Computer Engineering Technology (Computer Systems)  
Universiti Kuala Lumpur  

This project reflects my academic learning journey in Artificial Intelligence and Computer Vision.
