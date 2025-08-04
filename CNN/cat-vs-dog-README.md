
# 🐶 Dog vs Cat Classifier (CNN - Keras, TensorFlow)

This project builds a Convolutional Neural Network (CNN) using Keras and TensorFlow to classify images of cats and dogs from the Kaggle dataset.

## 🔧 Features
- Trains a CNN with multiple Conv2D + MaxPooling2D layers
- Uses `ImageDataGenerator` for image preprocessing and augmentation
- Includes `EarlyStopping` and `ModelCheckpoint` to save the best performing model (`best_model.h5`)
- Visualizes predictions: plots test images with true vs predicted labels
  - Green title = correct prediction
  - Red title = incorrect prediction

## 📁 Dataset
- Dataset path: `/kaggle/input/dog-vs-cat/animals/`
- Folder structure:
  ```
  /cat/*.jpg
  /dog/*.jpg
  ```

## 📦 Outputs
- `best_model.h5`: CNN model saved when highest validation accuracy is achieved
- Accuracy printed at the end of training
- Mixed cat and dog test predictions plotted with prediction correctness

## 🚀 How to Use
1. Upload this notebook to [Kaggle](https://www.kaggle.com/)
2. Attach the **Dog vs Cat** dataset via the "Add Data" sidebar
3. Enable "Internet" if you want to push results to GitHub
4. Run all cells in order

## 📜 Requirements
- TensorFlow / Keras
- Matplotlib
- Pandas / NumPy
- scikit-learn

---

Made with ❤️ for binary image classification.
