# Diabetic Retinopathy Classification Using CNN

This project implements a Convolutional Neural Network (CNN) to classify retinal images based on the severity of diabetic retinopathy. The dataset used is from a Kaggle competition and includes high-resolution images labeled with five categories of diagnosis.

## 🔍 Problem Statement

Diabetic Retinopathy (DR) is one of the leading causes of blindness in the working-age population. Early detection and classification into correct stages are crucial for treatment and management. This model aims to classify images into the following five classes:

- **No_DR**: No signs of diabetic retinopathy  
- **Mild**: Mild non-proliferative DR  
- **Moderate**: Moderate non-proliferative DR  
- **Severe**: Severe non-proliferative DR  
- **Proliferate_DR**: Proliferative diabetic retinopathy

## 📁 Dataset

- **Source**: [Kaggle Diabetic Retinopathy Dataset](https://www.kaggle.com)
- **Preprocessing**:
  - Images resized to `200x200`
  - Labels mapped to class names
  - Images organized into folders by class using `os` module
  - Train-test split performed on original CSV

## 🧠 Model Architecture

- **Model Type**: CNN using `TensorFlow` and `Keras`
- **Augmentation**: Used `ImageDataGenerator` to apply:
  - Rescaling
  - Rotation
  - Zoom
  - Shearing
  - Flipping
- **Loss Function**: Categorical Crossentropy
- **Optimizer**: Adam
- **Metrics**: Accuracy

## 📈 Training & Evaluation

- Model trained on ~2000 images
- Validation performed on a separate set
- Highest accuracy model saved using `model.save()`
- Visualization using `matplotlib` to compare predictions vs true labels
- Subplots display green titles for correct predictions and red for incorrect ones

## 🖼️ Visualization

Predictions are visualized using 4x4 grid subplots to display:
- True label
- Predicted label
- Correctness (color-coded)

## 💾 How to Use

```bash
# Install dependencies
pip install tensorflow pandas numpy matplotlib

# Run the notebook or script to train the model
python train_model.py

# To visualize predictions
python show_predictions.py
