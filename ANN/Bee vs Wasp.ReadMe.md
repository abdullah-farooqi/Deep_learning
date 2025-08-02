# Multi-Class Image Classification using CNN

This project implements a Convolutional Neural Network (CNN) to classify images into multiple categories using TensorFlow and Keras. It includes data preprocessing, model training, evaluation, and visualization of results.

## 📁 Project Structure
- `train_df`, `val_df`, `test_df`: Pandas dataframes containing image paths and corresponding labels.
- `train_generator`, `val_generator`, `test_generator`: Keras generators created using `ImageDataGenerator` for efficient loading and augmentation.
- CNN architecture: Custom sequential CNN model with BatchNormalization, Dropout, and ReLU activations.
- Transfer Learning (optional): The model can be extended to use pre-trained networks such as VGG16 or ResNet.
- Visualization: Training and validation accuracy/loss plots, and image predictions displayed alongside true labels.

## 🧠 Features
- Multi-class classification (e.g., 3 or more classes)
- Real-time data augmentation
- Model performance visualization
- Early stopping and learning rate reduction callbacks
- Scalable for use with larger datasets and models

## ✅ Requirements
- Python 3.x
- TensorFlow / Keras
- Pandas
- NumPy
- Matplotlib

Install dependencies with:
```bash
pip install tensorflow pandas numpy matplotlib
