# MNIST Handwritten Digit Recognizer using Deep CNN

## About the Experiment

This project implements a Deep Convolutional Neural Network (CNN) using TensorFlow and Keras to recognize handwritten digits from the MNIST dataset.

The model learns patterns from handwritten images and classifies them into one of the 10 digits from 0 to 9.

## Objective

To design, implement, train, and evaluate a Deep Convolutional Neural Network for handwritten digit recognition using the MNIST dataset.

The experiment also demonstrates the use of:

- Convolutional layers
- ReLU activation function
- Max Pooling
- Flattening
- Dense layers
- Softmax activation
- Adam optimizer
- Loss function
- Model training and evaluation

## Dataset

The MNIST dataset contains handwritten images of digits from 0 to 9.

- Training images: 60,000
- Testing images: 10,000
- Image size: 28 × 28 pixels
- Image type: Grayscale
- Number of classes: 10 (0–9)

The dataset is loaded directly using TensorFlow/Keras.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- MNIST Dataset
- Google Colab / Jupyter Notebook

## CNN Architecture

The CNN used in this experiment consists of the following layers:

1. Conv2D - 32 filters of size 3 × 3 with ReLU activation
2. MaxPooling2D - 2 × 2 pooling
3. Conv2D - 64 filters of size 3 × 3 with ReLU activation
4. MaxPooling2D - 2 × 2 pooling
5. Flatten layer
6. Dense layer - 64 neurons with ReLU activation
7. Dense output layer - 10 neurons with Softmax activation

### Model Flow

Input Image (28 × 28 × 1)
        ↓
Conv2D (32 filters)
        ↓
MaxPooling
        ↓
Conv2D (64 filters)
        ↓
MaxPooling
        ↓
Flatten
        ↓
Dense (64 neurons)
        ↓
Dense (10 neurons)
        ↓
Predicted Digit (0–9)

## Data Preprocessing

The MNIST images are originally represented using pixel values from 0 to 255.

The images are reshaped into:

```text
28 × 28 × 1

## 👤 Author

**Jishan Attar**  
