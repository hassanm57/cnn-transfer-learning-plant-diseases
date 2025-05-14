# 🌿 Plant Disease Classification using CNN & Transfer Learning

This project applies deep learning techniques to accurately classify plant leaf diseases using transfer learning on well-known CNN architectures like ResNet50 and Xception. The models were trained on a Kaggle dataset of labeled plant leaf images and evaluated using a separate test set.

---

## 📁 Dataset

- **Source**: [Kaggle Plant Village Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)
- **Train/Validation Split**: 80/20
- **Test Set**: Custom folder of 33 real-world images, with filenames indicating their true class (e.g., `TomatoHealthy1.JPG`, `PotatoEarlyBlight2.JPG`).

---

## 🧠 Models Used

### 1. **ResNet50**
- **Base frozen**: Custom classification head trained.
- **Top 25% layers unfrozen**: Fine-tuned on dataset.
- **Best Test Accuracy**: ~0.97

### 2. **Xception**
- **Base frozen**: Custom classification head trained.
- **Top 25% layers unfrozen**: Fine-tuned further.
- **Best Test Accuracy**: ~0.98

---

## 🧪 Results Summary

| Model         | Setting                | Test Accuracy | Test Loss |
|---------------|------------------------|---------------|-----------|
| ResNet50      | Base Frozen            | 0.9564        | 0.1458    |
| ResNet50      | Top 25% Unfrozen       | 0.9714        | 0.0895    |
| Xception      | Base Frozen            | 0.9352        | 0.1947    |
| Xception      | Top 25% Unfrozen       | 0.9848        | 0.0581    |

---

## 🧪 Evaluation on Test Set

Test set contains 33 real-world images. Ground truth is extracted from filenames and compared with predictions to generate metrics like:

- ✅ Accuracy
- 📉 Confusion Matrix
- 🧾 Classification Report

---

## 🧪 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/hassanm57/plant-disease-cnn](https://github.com/hassanm57/cnn-transfer-learning-plant-diseases.git
cd cnn-transfer-learning-plant-diseases
