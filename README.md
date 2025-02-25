# **Handwritten Arabic Character Recognition (CNN + Transfer Learning)**

## 📌 **Project Overview**
This project focuses on recognizing **handwritten Arabic characters** using **Transfer Learning** with **ResNet50**.  
The model was fine-tuned with a **custom head** and optimized using **hyperparameter tuning**.

- **Model Architecture**: ResNet50 + Custom Head
- **Dataset**: Arabic character dataset
- **Training Strategy**:
  - Transfer Learning with **ResNet50**
  - **Hyperparameter tuning** to optimize performance

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