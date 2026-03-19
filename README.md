# Age-Based Image Classification using CNN

A Deep Learning project designed to classify human faces into three categories: **Young, Middle, and Old**. This project utilizes a custom Convolutional Neural Network (CNN) architecture to process a dataset of approximately 19906 images.

---

## 🚀 Project Overview
This repository demonstrates a complete computer vision pipeline, from data preprocessing and augmentation to model training and evaluation. 

* **Dataset Size:** 19906 images
* **Categories:** Young, Middle, Old
* **Framework:** TensorFlow / Keras 

---

## 📊 Dataset & Preprocessing
The dataset consists of a `Images` folder containing images and a `Images&Labels.csv` file mapping filenames to their respective age labels.

### Data Handling:
- **Image Rescaling:** All images were normalized to a range of [0, 1].
- **Batch Processing:** Due to the 19k image count, I implemented a `DataGenerator` to load images in batches, ensuring efficient memory usage.
- **Augmentation:** Applied random rotations, flips, and zooms to improve model generalization.

> **Note:** The raw image dataset is not included in this repository due to size constraints. 
> [📥 Download Dataset from Google Drive](https://drive.google.com/drive/folders/1FM9MHlWi9rDTEq6ll-r3ct8XjPzWWT4s?usp=drive_link)

---

## 🧠 Model Architecture
I implemented a CNN with the following key components:
- **Convolutional Layers:** For feature extraction (edges, textures, facial patterns).
- **Max Pooling:** To reduce spatial dimensions and computational load.
- **Dropout Layers:** To prevent overfitting on the 19k training samples.
- **Output Layer:** Softmax activation for 3-class classification.

---

## 📈 Performance & Results
| Metric | Score |
| **Accuracy** | 76% |
| **Precision** | 72.3% |
| **Recall** | 79% |
