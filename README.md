[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/5HZkrI_Y)
[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/r8OAyKH-)
# CNN Classification Task with Cat-vs-Dog dataset

## Task Description
In this task,  will build a Convolutional Neural Network (CNN) for image classification. The goal is to classify images into two categories: **dogs** and **cats**. You will:

1. Preprocess and explore the dataset.
2. Build and train a CNN classification model.
3. Evaluate the model's performance using appropriate metrics.
4. Record your findings and observations under the **Findings** section.


## Dataset
The dataset used for this task is **Dogs vs. Cats**:

[Kaggle Dataset - Dog vs. Cat](https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset/data)

### Dataset Details:
- **Content**: Images of dogs and cats.
- **Format**: JPEG images.
- **Labels**: 0 for cat, 1 for dog.



1. **Model Requirements**:
   - Build a CNN model.
   - Include :
     - Input layer for image data.
     - Multiple convolutional layers with appropriate activation functions.
     - Pooling layers (e.g., MaxPooling).
     - Fully connected layers leading to a softmax or sigmoid output.
   - Use **binary cross-entropy** as the loss function for binary classification.

2. **Evaluation**:
   - Use metrics such as **accuracy**, **precision**, **recall**, and **F1-score**.
   - Create visualizations for:
     - Model training and validation loss.
     - Model training and validation accuracy.
     - Confusion matrix.



## Findings

---

## Model Architecture

The CNN model includes:

- **Input Layer:** (128 × 128 × 3)
- **Conv2D (32 filters) + ReLU**
- **MaxPooling**
- **Conv2D (64 filters) + ReLU**
- **MaxPooling**
- **Conv2D (128 filters) + ReLU**
- **MaxPooling**
- **Flatten**
- **Dense (256) + ReLU**
- **Dropout (0.5)**
- **Output Layer (Sigmoid)**

Loss Function: Binary Cross-Entropy


Optimizer: Adam (learning rate = 0.001)


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
- Accuracy : 0.8639
- Precision : 0.9084
- Recall : 0.8095
- F1-Score : 0.8561




### Classification Report:

          precision    recall  f1-score   support

Cat 0.83  0.92  0.87  2499 
Dog 0.91  0.81  0.86  2499

accuracy 0.86  4998



---



- The CNN achieved **86% accuracy** on the validation dataset.
- The model performs slightly better at detecting **cats** than **dogs**.
- **Dropout (0.5)** helped reduce overfitting.
- The learning rate **0.001** provided stable training.
- A **3-layer CNN architecture** was sufficient to achieve good classification performance.

---

## Visualizations


- Training vs Validation **Accuracy Curve**
- Training vs Validation **Loss Curve**
- **Confusion Matrix**

These visualizations help analyze model performance during training.

## References

The following Kaggle notebooks for guidance on loading
1. https://www.kaggle.com/code/uysimty/keras-cnn-dog-or-cat-classification
2. https://www.kaggle.com/code/prashant111/cnn-image-classification-cats-vs-dogs  
3. https://www.kaggle.com/code/chetankv/cnn-cats-vs-dogs-classification  
6. https://www.kaggle.com/code/uysimty/keras-cnn-dog-or-cat-classification