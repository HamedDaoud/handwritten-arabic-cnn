# **Handwritten Arabic Character Recognition (CNN + Transfer Learning)**

## 📌 **Project Overview**
This project focuses on recognizing **handwritten Arabic characters** using **Transfer Learning** with **ResNet50**.  
The model was fine-tuned with a **custom head** and optimized using **hyperparameter tuning**.

- **Model Architecture**: ResNet50 + Custom Head
- **Dataset**: Arabic character dataset
- **Training Strategy**:
  - Explored **multiple architectures** including **ResNet50** and **MobileNet**.
  - Designed and tested **various custom heads**.
  - Used **Keras Tuner** for **extensive hyperparameter tuning**.
  - Fine-tuned the best-performing models for **optimal accuracy**.

This project also served as a **learning playground** for implementing and applying key concepts in:
- **Transfer Learning**
- **Hyperparameter Tuning**
- **Convolutional Neural Networks (CNNs)**
- **TensorFlow & Keras**

---

## 🏆 **Key Results**
- **Performance Metrics**:
  - **Training Accuracy**: **99.22%**
  - **Validation Accuracy**: **94.52%**
  - **Best Model**: `arabic_letter_classifier_95_95`

- **Classification Report**:
  - Macro average F1-score: **0.95**
  - Weighted average F1-score: **0.95**
  - **Most misclassifications occurred between visually similar letters**.

- **Challenging Classes**:
  - The **lowest accuracy** was for **classes 56 and 57**.
  - These two classes represent **different writing variants of the same character**.
  - **Fixing these misclassifications** would lead to the model **memorizing specific writing styles**, which we **want to avoid** to maintain generalization.