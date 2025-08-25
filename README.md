# ✍️ CNN Handwriting Recognition

A **Convolutional Neural Network (CNN)** model to recognize handwritten digits from the **MNIST dataset**.  
This project demonstrates deep learning techniques for image classification with a creative architecture and visualization of training progress.

---

## 🚀 Project Overview

Handwriting recognition is a classic problem in machine learning and computer vision.  
This project uses CNNs to automatically extract features from images and classify handwritten digits (0-9) with high accuracy.

**Key Features:**
- Preprocessing of MNIST dataset
- CNN architecture with multiple layers
- Training & validation visualization
- Prediction of handwritten digits

---

## 🖼 Dataset

The model uses the **MNIST dataset**:
- 70,000 grayscale images of handwritten digits
- Image size: 28x28 pixels
- Training set: 60,000 images
- Test set: 10,000 images

---

## 🏗 CNN Architecture

| **Layer (Type)**                | **Output Shape**      | **Param #** |
|---------------------------------|--------------------|------------|
| Conv2D (conv2d)                 | (None, 26, 26, 32)  | 320        |
| MaxPooling2D (max_pooling2d)    | (None, 13, 13, 32)  | 0          |
| Conv2D (conv2d_1)               | (None, 11, 11, 16)  | 4,624      |
| MaxPooling2D (max_pooling2d_1)  | (None, 5, 5, 16)    | 0          |
| Flatten (flatten)                | (None, 400)         | 0          |
| Dense (dense)                    | (None, 100)         | 40,100     |
| Dense (dense_1)                  | (None, 10)          | 1,010      |

**Total parameters:** 46,054 (≈179.9 KB)  
**Trainable parameters:** 46,054 (≈179.9 KB)  
**Non-trainable parameters:** 0 (0.00 B)

---

## 📈 Training

- Loss function: **Sparse Categorical Crossentropy**
- Optimizer: **Adam**
- Metrics: **Accuracy**
- Epochs: 08 (adjustable)
- Batch size: 32 (default, can use 32–64)

---

## 🧪 Model Evaluation

After training the CNN on the dataset, the model was evaluated on the test set with the following results:

| Metric         | Value                |
|----------------|--------------------|
| **Test Loss**  | 0.0335             |
| **Test Accuracy** | 99.13%            |

> ⚡ The model achieved an impressive **99.13% accuracy**, demonstrating excellent performance in classifying the images with minimal error (loss ≈ 0.0335).  

This high accuracy shows that the CNN effectively learned the patterns in the dataset, making it highly reliable for predictions.

