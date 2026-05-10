# 📸 Natural Image Classification using CNN

[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)](https://www.tensorflow.org/)
[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)](https://www.python.org/)
[![Deep Learning](https://img.shields.io/badge/Deep-Learning-red)]()
[![CNN](https://img.shields.io/badge/CNN-Image%20Classification-success)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📌 Project Overview

This project implements a **Deep Learning Image Classification Model** using a **Convolutional Neural Network (CNN)** architecture to classify natural images into 8 different categories.

The project was developed as part of a Machine Learning course and demonstrates the complete workflow of building an image classification system, including preprocessing, augmentation, model training, evaluation, and deployment-ready model export.

---

## 🎯 Objectives
- Build an image classification model using CNN
- Understand deep learning workflow using TensorFlow/Keras
- Improve model generalization with image augmentation
- Evaluate model performance on unseen data
- Export trained models for deployment purposes

---

## 📝 Dataset Information

The dataset used is **Natural Images Dataset**, consisting of 8 categories:

- ✈️ Airplane
- 🚗 Car
- 🐱 Cat
- 🐶 Dog
- 🌸 Flower
- 🍎 Fruit
- 🏍️ Motorbike
- 👤 Person

### 📂 Data Split
The dataset was divided using `split-folders` with the following ratio:
- **80%** Training Data
- **10%** Validation Data
- **10%** Testing Data (Unseen Data)

---

## 🏗️ Model Architecture

The model was built using **TensorFlow Keras** with the following architecture components:

1. **Conv2D + MaxPooling2D**  
   Extract spatial features from input images.

2. **Dropout (0.5)**  
   Reduce overfitting and improve model generalization.

3. **Flatten + Dense Layer**  
   Convert extracted features into classification output.

4. **Activation Functions**
   - ReLU for hidden layers
   - Softmax for output layer (8 classes)

---

## ⚙️ Preprocessing & Data Augmentation

To improve model performance and generalization, several preprocessing techniques were applied:

- Rescaling pixel values to range **(0–1)**
- Image augmentation:
  - `rotation_range`
  - `horizontal_flip`
  - `shear_range`
- Image resizing to **150x150 pixels**

---

## 📊 Model Performance

The model achieved solid performance on validation and testing data:

- ✅ Validation Accuracy: **>85%**
- ✅ Test Accuracy: **>85%**

Training performance was monitored using:
- Accuracy graph
- Loss graph

These visualizations are included inside the notebook for transparency and evaluation purposes.

---

## 🚀 Deployment Ready

The trained model was exported into multiple formats for deployment flexibility:

- **TensorFlow SavedModel**
- **TensorFlow Lite (TFLite)** for mobile deployment
- **TensorFlow.js** for web deployment

---

## 📂 Project Structure

```text
.
├── saved_model/        # TensorFlow SavedModel format
├── tflite/             # TFLite model & labels
├── tfjs_model/         # TensorFlow.js model
├── requirements.txt    # Required libraries
├── proyek_akhir.ipynb  # Main notebook
└── README.md           # Project documentation
```

##🛠️ Tech Stack
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Google Colab / Jupyter Notebook

## ▶️ How to Run
1. Clone Repository

```bash
git clone https://github.com/imammularif/natural-image-classification.git
```

2. Install Dependencies

```bash
pip install -r requirements.txt
```

3. Open Notebook
Run proyek_akhir.ipynb using:
- Google Colab
- Jupyter Notebook


## 🧠 Key Learnings
- Building CNN-based image classification models
- Applying image preprocessing & augmentation
- Evaluating deep learning model performance
- Exporting models for deployment
- Understanding end-to-end deep learning workflow

## 🚀 Future Improvements
- Improve model accuracy with transfer learning
- Add confusion matrix visualization
- Optimize model size for deployment
- Build web interface for real-time predictions

## 👨‍💻 Author
- Imammul Arif
-📍 Indonesia
- 🔗 LinkedIn: https://linkedin.com/in/imammularif
- 🔗 GitHub: https://github.com/imammularif


