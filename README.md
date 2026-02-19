# CNN-Based Image Classification  
### Intel Image Classification Dataset

## Project Overview

This project implements a Convolutional Neural Network (CNN) for multi-class image classification using the Intel Image Classification Dataset.  

The model classifies natural scene images into six categories:
- Buildings
- Forest
- Glacier
- Mountain
- Sea
- Street

This project covers data preprocessing, CNN model development, training, evaluation, and performance visualization.

---

## Objective

To design, implement, and evaluate a CNN model for image classification using TensorFlow/Keras, including:

- Data preprocessing
- Data augmentation
- CNN architecture design
- Model training and validation
- Performance evaluation
- Prediction visualization

---

## Dataset

- **Dataset Name:** Intel Image Classification
- **Source:** Kaggle
- **Total Classes:** 6
- **Image Size Used:** 150 × 150
- **Dataset Split:**
  - Training: 80%
  - Validation: 20%
  - Test: Separate test folder

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab (GPU)

---

## Data Preprocessing

The following preprocessing steps were applied:

- Resizing images to 150×150
- Pixel value normalization (0–255 → 0–1)
- Train-validation split (80-20)
- Data augmentation:
  - Random horizontal flip
  - Random rotation
  - Random zoom

Data augmentation improves model generalization and reduces overfitting.

---

## CNN Architecture

The CNN model includes:

- 3 Convolutional Layers (ReLU activation)
- MaxPooling layers
- Flatten layer
- Fully Connected (Dense) layer
- Dropout (0.5) for regularization
- Output layer with Softmax activation (6 classes)

### Model Flow:

Input Image  
→ Rescaling  
→ Data Augmentation  
→ Conv2D + ReLU  
→ MaxPooling  
→ Conv2D + ReLU  
→ MaxPooling  
→ Conv2D + ReLU  
→ MaxPooling  
→ Flatten  
→ Dense (128)  
→ Dropout  
→ Output (Softmax)

---

## Training Details

- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Metrics: Accuracy
- Callbacks:
  - Early Stopping
  - Model Checkpoint

---

## Model Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score (per class)
- Confusion Matrix

Training and validation accuracy/loss curves were plotted to analyze overfitting.

---

## Results

- Achieved strong classification performance across six classes.
- Confusion matrix analysis showed minor misclassifications between similar classes (e.g., Glacier vs Mountain).
- Data augmentation improved validation accuracy.

---

## Prediction Visualization

Random test images were displayed with:
- Predicted Label
- Actual Label

This helped interpret model performance visually.

---

## Future Improvements

- Use Transfer Learning (MobileNetV2 / ResNet50)
- Hyperparameter tuning
- Batch Normalization
- Learning rate scheduling
- Fine-tuning pretrained models

---

## Conclusion

This project demonstrates the complete workflow of building a CNN from scratch for image classification.  

It provides practical understanding of:
- Convolutional Neural Networks
- Model training and evaluation
- Overfitting control
- Performance analysis

---

## Author

**Fathima Salga**  
Deep Learning Enthusiast | Data Science Learner
