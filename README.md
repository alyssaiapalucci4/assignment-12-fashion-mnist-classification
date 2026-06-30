# Fashion-MNIST Image Classification using Neural Networks

## Project Overview
This project demonstrates image classification using a feedforward neural network trained on the Fashion-MNIST dataset. The goal is to classify grayscale images of clothing items into 10 categories such as shirts, shoes, dresses, and bags.

The project compares traditional deep learning architecture (MLP) performance on image classification tasks and demonstrates the full pipeline from data preprocessing to model evaluation.

---

## Dataset
The dataset used is the Fashion-MNIST dataset:
- 70,000 grayscale images (28×28 pixels)
- 10 clothing categories
- 60,000 training images and 10,000 test images

Classes:
- T-shirt/top  
- Trouser  
- Pullover  
- Dress  
- Coat  
- Sandal  
- Shirt  
- Sneaker  
- Bag  
- Ankle boot  

---

## Model Architecture
A simple feedforward neural network (Multilayer Perceptron) was used:

- Flatten layer (28×28 → 784)
- Dense layer (128 neurons, ReLU activation)
- Dense layer (64 neurons, ReLU activation)
- Output layer (10 neurons, Softmax activation)

---

## Training Configuration
- Optimizer: Adam  
- Loss Function: Sparse Categorical Crossentropy  
- Batch Size: 32  
- Epochs: 15  
- Validation Split: 20%  

---

## Data Preprocessing
- Pixel values normalized from 0–255 to 0–1
- Optional data augmentation applied (rotation, shift, zoom)

---

## Evaluation Metrics
The model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

---

## Results
The model achieved reasonable classification performance on the test set.

Key observations:
- High accuracy on clearly distinct classes (e.g., bags, boots)
- Lower accuracy on visually similar classes (e.g., shirts vs T-shirts)
- Confusion matrix highlights common misclassifications

---

## Visualizations
The project includes:
- Training vs validation accuracy graph
- Training vs validation loss graph
- Confusion matrix heatmap

---

## Application
This model can be used in real-world applications such as:
- Automated product tagging in fashion e-commerce platforms
- Image-based search systems
- Inventory classification in retail warehouses

---

## Limitations
- Feedforward neural networks do not capture spatial image features as effectively as CNNs
- Dataset images are low-resolution and simplified compared to real-world data
- Model performance may decrease on complex real-world images

---

## Future Improvements
- Implement Convolutional Neural Networks (CNNs)
- Apply stronger data augmentation techniques
- Perform hyperparameter tuning
- Deploy as a web or mobile application using an API

---

## How to Run
1. Open the Jupyter/Colab notebook
2. Install required libraries:
   ```bash
   pip install tensorflow numpy matplotlib seaborn scikit-learn
3. Run all cells from top to bottom
4. View evaluation results and visualizations
   
---

--- 

Author

Alyssa I

---
