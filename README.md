# Morphed Face Image Detection Using PCA and Machine Learning

## Overview

Face recognition systems are widely used in biometric authentication, but they are vulnerable to face morphing attacks where two facial images are blended to create a manipulated identity. This project presents a machine learning-based solution to detect morphed face images using Principal Component Analysis (PCA) and classification algorithms.

The system extracts important facial features using PCA and classifies images as **Original** or **Morphed** using machine learning models such as **SVM, KNN, Decision Tree, and Logistic Regression**.

---

## Objectives

* Detect morphed face images used in biometric spoofing attacks.
* Extract discriminative facial features using PCA.
* Reduce image dimensionality for efficient processing.
* Compare multiple machine learning classifiers.
* Improve the security and reliability of biometric authentication systems.

---

## Dataset

**Dataset:** Real and Fake Face Detection

**Source:** Kaggle (CIPLab, Yonsei University, South Korea)

### Dataset Statistics

* Total Images: 2,041
* Original Images: 1,081
* Morphed Images: 960
* Original Resolution: 600 × 600 pixels
* Classes: Original (0), Morphed (1)

---

## Technologies Used

* Python
* OpenCV
* NumPy
* Scikit-learn
* Matplotlib
* Joblib
* Google Colab

---

## Methodology

### 1. Data Collection

* Downloaded dataset from Kaggle.
* Organized images into Original and Morphed classes.

### 2. Image Preprocessing

* Resize images to 64 × 64 pixels.
* Convert images to grayscale.
* Normalize pixel values.
* Flatten images into feature vectors.

### 3. Feature Extraction

* Apply Principal Component Analysis (PCA).
* Reduce dimensionality while preserving important facial information.
* Generate Eigenfaces and PCA projections.

### 4. Model Training

The following classifiers were trained and evaluated:

* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)
* Decision Tree
* Logistic Regression

### 5. Image Classification

* Process new facial image.
* Apply PCA transformation.
* Predict whether the image is Original or Morphed.

---

## Project Workflow

Dataset → Preprocessing → PCA Feature Extraction → Model Training → Classification → Prediction

---

## Results

* PCA successfully reduced image dimensionality.
* Multiple machine learning models were evaluated.
* Support Vector Machine (SVM) achieved the best performance and was selected as the final model.
* The system effectively distinguishes original and morphed facial images.

---

## Installation

```bash
pip install numpy pandas matplotlib opencv-python scikit-learn joblib
```

---

## Run the Project

```bash
jupyter notebook
```

Open:

```text
Morphed_Face_Detection.ipynb
```

Run all cells to train and test the model.

---

## Future Enhancements

* Deep Learning based morph detection using CNNs.
* Real-time morph detection system.
* Integration with biometric authentication platforms.
* Improved performance using larger datasets.
