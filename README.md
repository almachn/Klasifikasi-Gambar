# 🐾 Dog Breed Classifier with CNN (TensorFlow/Keras)

This is a deep learning project that classifies dog breeds using a Convolutional Neural Network (CNN) model built with TensorFlow/Keras. The dataset contains over 10,000 images spanning 25 dog breeds. Woof!

## 🧠 Features
- Image classification using CNN
- Trained on a custom dog breed dataset
- Achieves high accuracy on both training and validation
- Exported to `.h5`, `.tflite`, and TensorFlow.js formats for deployment
- Inference support for custom images via saved model

---

## 🗂️ Dataset
- Source: [Dog Breeds Dataset on Kaggle](https://www.kaggle.com/datasets/imbikramsaha/dog-breeds)



---

## 🏗️ Model Architecture
- Input Layer (128x128 RGB image)
- 3x Conv2D + MaxPooling layers
- Flatten + Dense + Dropout
- Output Layer with 25 units (softmax)

---

## 🚀 How to Use

### 🔧 Installation
You can install all the dependencies with:

```bash
pip install -r requirements.txt
```
### 🏃‍♂️ Run Inference
predicted_label, confidence = predict_savedmodel(
    img_path="/path/to/dog/image.jpg", 
    model=model, 
    class_names=class_names
)

(Inference via CLI (Colab))
img_path = input("Masukkan path gambar untuk prediksi: ")
predict_savedmodel(img_path, model, class_names)

### 📦 Exported Formats
- model.h5 — Keras HDF5 model

- model.tflite — TensorFlow Lite

- tfjs_model/ — TensorFlow.js format

- labels.txt — List of class names (25 dog breeds)
