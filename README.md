# 🌱 Plant Disease Detection using CNN & MobileNetV2

This project focuses on **classifying plant leaves** into **Healthy vs Diseased** categories using Deep Learning.  
We experimented with a **Custom CNN** and **MobileNetV2 (Transfer Learning)** to evaluate performance.  

---

## 📌 Problem Statement
Plant diseases affect crop yield and food security worldwide.  
An **automated leaf disease detection system** can help farmers take timely actions and reduce crop loss.  

---

## 📊 Dataset
- **Source:** [PlantVillage Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)  
- Images were reorganized into two categories:
  - `Healthy`
  - `Diseased`  

Dataset was split into:
- **Train (80%)**
- **Validation (10%)**
- **Test (10%)**

---

## 🧠 Models Implemented
### 1️⃣ Custom CNN
- 2 Convolutional layers
- MaxPooling, Dropout for regularization
- Dense layers for classification

### 2️⃣ MobileNetV2 (Transfer Learning)
- Pretrained on ImageNet
- Feature extractor with GlobalAveragePooling
- Fine-tuned Dense layers

---

## 📈 Results
| Model        | Accuracy | Precision | Recall | F1-score |
|--------------|----------|-----------|--------|----------|
| CNN          | ~0.79    | ~0.78     | ~0.80  | ~0.79    |
| MobileNetV2  | ~0.98    | ~0.97     | ~0.98  | ~0.98    |

✅ MobileNetV2 significantly outperformed the baseline CNN.  

---

## 🔥 Grad-CAM Visualization
To improve explainability, we applied **Grad-CAM** to highlight regions that contributed to the prediction.  

Example (Healthy vs Diseased leaf):
![Grad-CAM Example](gradcam_example.png)

---

## 🛠️ Requirements
```bash
Python 3.x
TensorFlow / Keras
NumPy
Pandas
Matplotlib
Seaborn
scikit-learn
OpenCV

