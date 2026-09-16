# MNIST Handwritten Digit Recognizer using Deep CNN

This project implements a Deep Convolutional Neural Network (CNN) to recognize handwritten digits. Built using TensorFlow and Keras, the model analyzes grayscale images from the MNIST dataset and classifies them into one of the 10 digits, from 0 to 9.

## 🚀 Tech Stack & Libraries

- **Deep Learning Framework:** TensorFlow, Keras
- **Data Manipulation & Analysis:** NumPy
- **Data Visualization:** Matplotlib
- **Dataset:** MNIST
- **Development Environment:** Google Colab / Jupyter Notebook

## 📊 Dataset Information

- **Dataset:** MNIST Handwritten Digits Dataset
- **Training Images:** 60,000
- **Testing Images:** 10,000
- **Image Size:** 28 × 28 pixels
- **Image Type:** Grayscale
- **Number of Classes:** 10 (0–9)

## ⚙️ Data Preprocessing

1. **Reshaping:** Reshaped the images into `28 × 28 × 1` format to provide the grayscale channel required by the CNN.
2. **Normalization:** Divided pixel values by `255` to convert them from the range `0–255` to `0–1`.
3. **Dataset Loading:** Loaded the MNIST dataset directly using TensorFlow/Keras.

## 🧠 Model Architecture

The Deep Convolutional Neural Network is built using a sequential stack:

- **Convolutional Layer 1:** 32 filters of size `3 × 3` with `ReLU` activation
- **Max Pooling Layer 1:** `2 × 2` pooling
- **Convolutional Layer 2:** 64 filters of size `3 × 3` with `ReLU` activation
- **Max Pooling Layer 2:** `2 × 2` pooling
- **Flatten Layer:** Converts feature maps into a one-dimensional array
- **Dense Layer:** 64 neurons with `ReLU` activation
- **Output Layer:** 10 neurons with `Softmax` activation

## 🏃‍♂️ Training Details

- **Optimizer:** Adam
- **Loss Function:** Sparse Categorical Crossentropy
- **Metrics:** Accuracy
- **Epochs:** 10
- **Batch Size:** 64
- **Validation Split:** 10%

## 📈 Evaluation & Results

- **Test Evaluation:** The trained model is evaluated using the MNIST test dataset.
- **Accuracy Visualization:** Training and validation accuracy are plotted across all epochs.
- **Loss Visualization:** Training and validation loss are plotted to observe model performance.
- **Prediction Visualization:** The predicted and actual labels of the first 10 test images are displayed.

The model achieved approximately **99.07% accuracy** on the unseen testing data.

## 👤 Author

**Jishan Attar**
