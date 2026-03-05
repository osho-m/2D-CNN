# 2D-CNN — CIFAR-10 Image Classification

A deep learning project that implements a **2D Convolutional Neural Network (CNN)** to classify images from the CIFAR-10 dataset into 10 distinct categories using Keras and TensorFlow.

---

## 📌 Project Overview

The CIFAR-10 dataset contains 60,000 colour images (32×32 pixels) across 10 classes. This project builds, trains, and evaluates a multi-layer CNN to accurately classify these images using convolutional feature extraction and regularisation techniques.

**Classes:** airplane · automobile · bird · cat · deer · dog · frog · horse · ship · truck

---

## 🧠 Model Architecture

The CNN is built using Keras Sequential API with the following layers:

| Layer | Details |
|---|---|
| Conv2D | Convolutional layer for feature extraction |
| MaxPool2D | Max pooling for spatial downsampling |
| Dropout | Regularisation to prevent overfitting |
| Flatten | Converts 2D feature maps to 1D vector |
| Dense | Fully connected layers for classification |

**Optimiser:** SGD (Stochastic Gradient Descent)  
**Loss Function:** Categorical Crossentropy  
**Callbacks:** EarlyStopping, ModelCheckpoint

---

## 🛠️ Tech Stack

- Python 3.x
- Keras / TensorFlow
- NumPy
- Matplotlib

---

## 📁 Project Structure

```
2D-CNN/
│
└── Code/
    └── CIFAR_10_2D_CNN.ipynb   # Main notebook with full pipeline
```

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install tensorflow keras numpy matplotlib
```

### Run the Notebook

```bash
jupyter notebook Code/CIFAR_10_2D_CNN.ipynb
```

---

## 📊 Workflow

1. **Load Libraries** — Keras, NumPy, Matplotlib
2. **Load Dataset** — CIFAR-10 via `keras.datasets`
3. **Explore Data** — Visualise sample images and class distribution
4. **Preprocess** — Normalise pixel values, one-hot encode labels
5. **Build Model** — Define CNN architecture using Sequential API
6. **Train Model** — Fit with EarlyStopping and ModelCheckpoint callbacks
7. **Evaluate** — Assess accuracy and loss on test set
8. **Visualise Results** — Plot training/validation curves

---

## 📈 Sample Output

Example training images from the dataset:

| Label Index | Class |
|---|---|
| 0 | airplane |
| 1 | automobile |
| 2 | bird |
| 3 | cat |
| 4 | deer |
| 5 | dog |
| 6 | frog |
| 7 | horse |
| 8 | ship |
| 9 | truck |

---

## 🔍 Key Concepts Demonstrated

- **Convolutional Feature Extraction** — Using Conv2D layers to detect spatial patterns
- **Regularisation** — Dropout layers to reduce overfitting
- **Callbacks** — EarlyStopping to avoid overtraining; ModelCheckpoint to save best weights
- **Data Preprocessing** — Pixel normalisation and one-hot encoding
- **Multi-class Classification** — Softmax output over 10 categories

---

## 📚 Dataset Reference

- [CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html) — Krizhevsky, 2009
- Loaded directly via `keras.datasets.cifar10`

---

## 👤 Author

**Osho Muralidaran**  
[LinkedIn](https://www.linkedin.com/in/osho-m) · [GitHub](https://github.com/osho-m)
