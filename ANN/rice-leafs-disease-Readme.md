# 🌾 Rice Leaf Disease Classification using CNN

This project focuses on detecting and classifying rice leaf diseases using deep learning (CNN) techniques. A custom convolutional neural network was trained on a dataset containing six categories of rice leaf conditions.

## 📁 Dataset

The dataset contains **2,627 images** across the following 6 classes:

- Bacterial Leaf Blight
- Brown Spot
- Healthy
- Leaf Blast
- Leaf Scald
- Narrow Brown Spot

The data is organized into:
- `train/`: Training images (in class-wise subfolders)
- `validation/`: Validation images (in class-wise subfolders)

Data was loaded and labeled using `pandas` DataFrames and `ImageDataGenerator.flow_from_dataframe()`.

## 🧠 Model Architecture

A custom Convolutional Neural Network (CNN) was built using **TensorFlow/Keras**, featuring:

- Multiple `Conv2D` and `MaxPooling2D` layers
- Dropout for regularization
- `Dense` layers for final classification
- `softmax` activation in the output layer

The model was trained with:
- `categorical_crossentropy` loss
- `Adam` optimizer
- Accuracy as the evaluation metric

## 📈 Training Performance

The model was trained over 50 epochs and achieved:

- **Final Validation Accuracy**: ~92%
- Training/Validation accuracy and loss plots are included for visualization.

## 🔍 Evaluation

Despite high validation accuracy, manual testing revealed poor performance on some external images — likely due to:
- Preprocessing differences (e.g., missing normalization)
- Differences in image quality/distribution
- Label mismatch during manual mapping

This emphasizes the importance of **consistent preprocessing** and **thorough testing**.

## 🛠️ Future Improvements

- Use **transfer learning** (e.g., with MobileNetV2 or EfficientNet)
- Apply stronger **data augmentation**
- Add **early stopping** and **learning rate scheduling**
- Evaluate on a **separate test set**

## 📎 Resources

Dataset: Collected from the internet and cleaned manually  
Deep Learning Framework: TensorFlow / Keras  
Notebook: Kaggle

---

📌 For more updates and similar projects, visit:  
🔗 [My GitHub](https://github.com/abdullah-farooqi/Deep_learning.git)
