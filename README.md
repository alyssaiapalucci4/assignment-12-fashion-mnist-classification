# Fashion-MNIST Image Classification using Neural Networks

## Overview

This project implements a **feedforward neural network (MLP)** to classify images from the Fashion-MNIST dataset into 10 clothing categories.


---

## Dataset

- 70,000 grayscale images (28×28 pixels)
- 10 clothing categories (e.g., shirts, shoes, bags, dresses)
- Source: TensorFlow/Keras dataset

---

## Methodology

### Data Loading & Visualization

- Dataset loaded using TensorFlow/Keras
- Sample images displayed per class for exploration


### Preprocessing

- Pixel normalization to range [0,1]
- Data augmentation (rotation, shift, zoom) implemented and visualized but **not used in training**

---

## Model Architecture

- Flatten (28×28 → 784)
- Dense layer (128 neurons, ReLU)
- Dense layer (64 neurons, ReLU)
- Output layer (10 neurons, Softmax)

---

## Training Setup

- Optimizer: Adam
- Loss: Sparse Categorical Crossentropy
- Epochs: 15
- Batch size: 32
- Validation split: 20%

---

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The model performs well on distinct classes but struggles with visually similar categories.

---

## Application

This model can be used in:
- Fashion retail product tagging
- Image-based search systems
- Automated inventory classification

### Challenges
- Scalability for large-scale deployment
- Real-time inference requirements
- Real-world image variability (lighting, background noise)

---

## Future Improvements

- Replace MLP with CNN for better feature extraction
- Apply augmentation during training
- Hyperparameter tuning
- Optimize for deployment (mobile/cloud)

---

## Tech Stack

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## How to Run
1. Open the Jupyter/Colab notebook: Assignment_12_AI.ipynb
2. Install required libraries:
   ```bash
   pip install tensorflow numpy matplotlib seaborn scikit-learn
3. Run all cells from top to bottom
4. View evaluation results and visualizations 

---

## Author
Alyssa I

---

## Notes
- Augmentation was implemented and visualized but not used in final training
- Project built for educational purposes
