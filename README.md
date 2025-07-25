# 🧠 Practical Implementation of CNN with CIFAR-10

This project demonstrates how to build, train, and evaluate a **Convolutional Neural Network (CNN)** using TensorFlow and Keras on the popular **CIFAR-10** image classification dataset.

---

## 📂 Dataset: CIFAR-10

- CIFAR-10 is a dataset of 60,000 32x32 color images.
- It has **10 classes**:  
  `airplane`, `automobile`, `bird`, `cat`, `deer`, `dog`, `frog`, `horse`, `ship`, `truck`.

---

## 🏗️ Model Architecture

A simple CNN built using Keras Sequential API:

1. `Conv2D` layer with 32 filters (3x3 kernel), ReLU activation
2. `MaxPooling2D` to reduce spatial size
3. `Conv2D` with 64 filters → `MaxPooling2D` → another `Conv2D`
4. `Flatten` to convert feature maps to 1D
5. `Dense` (fully connected) layer with 64 units
6. Final `Dense` layer with 10 units (1 for each class)

---

## 🔧 How to Run

1. Install dependencies:
    ```bash
    pip install tensorflow matplotlib
    ```

2. Run the notebook:
    ```bash
    jupyter notebook Practical\ implimentation\ of\ cnn.ipynb
    ```

---

## 📊 Training

- The model is trained for **10 epochs**.
- Uses **Adam optimizer** and **Sparse Categorical Crossentropy loss**.
- Plots training and validation accuracy for monitoring.

---

## 🧪 Evaluation

- After training, the model is evaluated on the test set.
- Accuracy is printed and compared visually using plots.

---

## 📈 Sample Accuracy Achieved

```txt
Test Accuracy: ~0.70 - 0.75 (may vary slightly per run)
