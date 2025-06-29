# 🐶 Dogs vs. 🐱 Cats - Image Classification Project

This project explores **binary image classification** for cats and dogs using three different modeling approaches:

1. ✅ Random Forest (with and without PCA)
2. ✅ Custom Convolutional Neural Network (CNN)
3. ✅ Pre-trained VGG16 using Transfer Learning + Fine-Tuning

---

## 📊 Dataset
We use a subset of the Kaggle [Dogs vs. Cats dataset](https://www.kaggle.com/competitions/dogs-vs-cats/data), containing:

- 1,000 training images
- 100 testing images
- Balanced classes (50% dogs, 50% cats)

---

## 🛠 Tools & Libraries

- Python 3.x
- TensorFlow / Keras
- scikit-learn
- matplotlib / seaborn
- NumPy / pandas

---

## 📈 Results Overview

| Model                  | Validation Accuracy | Validation Loss |
|------------------------|---------------------|------------------|
| Random Forest (raw)    | 63.00%              | -                |
| Random Forest + PCA    | 59.20%              | -                |
| Custom CNN             | 72.00%              | 0.5461           |
| Frozen VGG16           | 89.00%              | 0.2394           |
| Fine-tuned VGG16       | 94.50%              | 0.1698           |

---

## 🧠 Key Insights

- Classical models like **Random Forest** perform poorly on raw pixel data.
- A **Custom CNN** improves performance but requires careful regularization.
- **Transfer Learning** with VGG16 achieves the highest accuracy and generalization, even with limited training data.

---

## 📂 Project Structure

- `notebooks/` – Jupyter notebook with full model pipeline
- `models/` – Saved Keras model files
- `results/` – Accuracy and loss plots
- `data/sample_images/` – A few example dog/cat images

---

## 🚀 Future Work

- Train on the full 25k Kaggle dataset
- Explore model ensembling (CNN + VGG16)
- Try ResNet50 or EfficientNet
- Improve training with early stopping, learning rate scheduling
