# 🌾 Paddy Leaf Disease Detection Using Deep Learning

## 📌 Overview

This project implements a deep learning-based image classification system to detect paddy leaf diseases using **Transfer Learning**. The model classifies paddy leaf images into four disease categories using a fine-tuned **MobileNetV2** architecture.

This system aims to assist in early detection of crop diseases to improve agricultural productivity and reduce manual inspection effort.

---

## 🎯 Objectives

- Detect and classify paddy leaf diseases automatically
- Apply transfer learning using MobileNetV2
- Improve model generalization using data augmentation
- Evaluate model performance using accuracy and confusion matrix
- Prevent overfitting through regularization techniques

---

## 🧠 Model Architecture

- **Base Model:** MobileNetV2 (Pretrained on ImageNet)
- **Custom Classification Head:**
  - GlobalAveragePooling2D
  - Dense Layer (ReLU)
  - Dropout Layer
  - Softmax Output Layer (4 Classes)

---

## 🏗 Project Structure

```
paddy-leaf-disease-detection/
│
├── data/
│   ├── train/
│   └── validation/
│
├── notebooks/
│   └── training.ipynb
│
├── models/
│   └── best_model.h5
│
├── src/
│   ├── train.py
│   ├── predict.py
│   ├── preprocessing.py
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Technologies Used

- Python
- TensorFlow / Keras
- MobileNetV2
- Keras Tuner
- NumPy
- Matplotlib
- Scikit-learn
- OpenCV

---

## 📊 Model Performance

- Training Accuracy: ~99%
- Validation Accuracy: ~98–99%
- Evaluation Metrics:
  - Accuracy
  - Confusion Matrix
  - Precision
  - Recall

---

## 🗂 Dataset Structure

```
data/
 ├── train/
 │   ├── Disease_1/
 │   ├── Disease_2/
 │   ├── Disease_3/
 │   ├── Disease_4/
 └── validation/
```

---

## 🔄 Data Preprocessing & Augmentation

- Rescaling (1./255)
- Random Rotation
- Zoom Augmentation
- Horizontal Flip
- Image Resizing (224x224)

---

## 🚀 How to Run the Project

### 1️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 2️⃣ Train the Model

```bash
python src/train.py
```

### 3️⃣ Predict a New Image

```bash
python src/predict.py --image path_to_image.jpg
```

---

## 📈 Future Improvements

- Implement EarlyStopping & Learning Rate Scheduler
- Deploy model using Streamlit web app
- Convert model to TensorFlow Lite for mobile deployment
- Integrate real-time camera-based disease detection

---

## 👩‍💻 Author

**Nur Munawwarah Binti Muzamil**  
Bachelor of Computer Engineering Technology (Computer Systems)  
AI & Machine Learning Enthusiast  

📧 Email: nurmunawwarah1@gmail.com  
🔗 LinkedIn: linkedin.com/in/nurmunawwarah  

---

⭐ If you found this project useful, feel free to give it a star!
