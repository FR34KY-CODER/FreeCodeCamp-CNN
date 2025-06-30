# 🐱🐶 Cat vs Dog Image Classifier - FreeCodeCamp Challenge (72% Accuracy)

This project is a **Convolutional Neural Network (CNN)** trained using TensorFlow 2 and Keras to classify images of cats and dogs — part of the [FreeCodeCamp Machine Learning Curriculum](https://www.freecodecamp.org/).

> 🔥 Final Accuracy: **72.0%** on a blind test set of 50 images  
> 🎯 Challenge Passed: ✅ Minimum requirement was 63% — **crushed it**

---

## 🚀 Features

- CNN built from scratch using `Sequential` API
- Trained on 2000 labeled images of cats and dogs
- Achieved 72% test accuracy without transfer learning
- Data augmentation to avoid overfitting
- Custom evaluation script that compares model outputs to a fixed answer key

---

## 🧪 Dataset

The dataset is automatically downloaded and unzipped from:
```https://cdn.freecodecamp.org/project-data/cats-and-dogs/cats_and_dogs.zip```

Directory structure:
```
cats_and_dogs/
├── train/
│ ├── cats/
│ └── dogs/
├── validation/
│ ├── cats/
│ └── dogs/
└── test/ # Unlabeled
```
## 📦 Dependencies

- TensorFlow 2.x
- Keras
- NumPy
- Matplotlib
Install using:

```
pip install tensorflow numpy matplotlib
```

## 🧠 Model Architecture
- Conv2D (32) → Conv2D (32) → MaxPooling  
- Conv2D (64) → Conv2D (64) → MaxPooling  
- Conv2D (128) → Conv2D (128) → MaxPooling  
- Flatten → Dense (256) → Dropout → Dense (1, Sigmoid)
- Optimizer: Adam (lr=0.0005)
- Loss: Binary Crossentropy
- Epochs: 20

## 📸 Sample Predictions
The model outputs probabilities for each test image (dog or cat), with visualizations:
```
🐶 92.34% dog  
🐱 76.45% cat  
```

## ✅ Challenge Result
```
Your model correctly identified 72.0% of the images of cats and dogs.
You passed the challenge!
```

## 👑 Author
Ojasvi Goyal (aka FR34K)
> Hardcore gamer, machine learning warrior, and code-slinger from LNMIIT, India.

## 🧠 Tips for Contributors
Want to improve it further?
- Try deeper CNNs or different data augmentation
- Convert to PyTorch for speed testing
- Build a Streamlit or Flask app for real-time image classification
