# Fighter Jet Image Classification Using Deep Learning

## 👨‍🎓 Student: Gaurav  
**Course**: Professional Certificate in Data Science  
**Platform**: Newton School  

## 🛠 Tools & Libraries
- Google Colab  
- TensorFlow / Keras  
- OpenCV  
- Matplotlib & Seaborn  

---

## 📌 Project Objective

This project aims to build a deep learning-based image classification system to automatically recognize and categorize different types of **fighter jets** using computer vision. Automating this task is crucial for enhancing **military surveillance, reconnaissance**, and **real-time threat detection** from camera feeds or satellite images.

---

## ❓ Problem Statement

To develop an AI model capable of **classifying fighter jet images** into predefined categories with **high accuracy**. The model should be able to **generalize well** on unseen data and reduce manual intervention in jet identification.

---

## 📂 Dataset Description

- **Source**: Fighter Planes Dataset  
- **Classes**:
  - F35
  - B52
  - Rafale
  - T50
  - U2  
- **Images**: ~800 images resized to **224x224** pixels  
- **Split**: 80% Training | 20% Testing  
- **Preprocessing**:
  - Normalization ([0,1] scaling)
  - One-hot encoding labels using `to_categorical`
  - `train_test_split` used for data split

---

## 🧠 Model Architecture

- **Type**: Custom Convolutional Neural Network (CNN)  
- **Layers**:
  - Conv2D → ReLU → MaxPooling → Dropout  
  - Flatten → Dense → Softmax  
- **Loss**: Categorical Crossentropy  
- **Optimizer**: Adam  
- **Evaluation Metric**: Accuracy

---

## 📊 Training & Evaluation

- **Epochs**: 10  
- **Batch Size**: 32  

| Metric         | Training Set | Validation Set |
|----------------|--------------|----------------|
| Accuracy       | ~99.38%      | ~40.90%        |
| Loss           | ~0.02        | Higher (overfitting) |
| Overfitting    | Yes (very high) |

- **Visualizations**:
  - Accuracy/Loss over Epochs  
  - Confusion Matrix  
  - Classification Report per Class  

---

## 💡 Insights & Business Value

- **High training accuracy** shows that the model is capable of learning.
- **Low validation accuracy** highlights the need for more data and model regularization.
- A solid baseline for **automated image classification** in **aerospace and defense**.
- Can be integrated with **real-time drone feeds** or **satellite imagery systems**.
  
---

## ⚠️ Limitations

- Small dataset size → Limited generalization  
- Similar aircraft silhouettes → Misclassification  
- Background noise and image quality impact accuracy  

---

## ✅ Recommendations

- Use **data augmentation** for better generalization  
- Apply **transfer learning** with pre-trained models (e.g., ResNet, VGG)  
- Add **regularization** (Dropout, L2)  
- Perform **hyperparameter tuning**  
- Introduce **early stopping** during training  

---

## 📁 Repository Contents

- 📓 `Jet_Classifier_Colab.ipynb` – Training notebook  
- 🧠 `plane_classifier_model.h5` – Trained model  
- 🖼️ `dataset/` – Fighter jet images  
- 📈 `results/` – Predictions and evaluation reports  
- 📄 `README.md` – Project overview  


---

## ✅ Conclusion

This project demonstrates the use of deep learning for **automated fighter jet classification**. Although the model shows signs of overfitting due to limited data, it provides a strong starting point. With enhancements like **transfer learning** and **data expansion**, this system has the potential to be deployed in **real-world defense and surveillance** operations.

---

