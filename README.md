# Animals-10 Image Classification using CNN and Transfer Learning

## Project Overview

This project was completed as part of the Ironhack AI Engineering Bootcamp.

The objective was to build an image classification model capable of recognizing ten different animal classes. The project compares a baseline Convolutional Neural Network (CNN) with a Transfer Learning approach using MobileNetV2.

---

## Dataset

The project uses the **Animals-10** dataset containing approximately **26,000 images** across the following classes:

- Dog (cane)
- Horse (cavallo)
- Elephant (elefante)
- Butterfly (farfalla)
- Chicken (gallina)
- Cat (gatto)
- Cow (mucca)
- Sheep (pecora)
- Spider (ragno)
- Squirrel (scoiattolo)

The dataset was split into:

- Training: 80%
- Validation: 10%
- Test: 10%

A stratified split was used to preserve the class distribution.

---

## Project Workflow

The project followed these steps:

1. Load and inspect the dataset
2. Explore class distribution
3. Visualize sample images
4. Preprocess the data
5. Build a baseline CNN
6. Improve the CNN using Dropout and Early Stopping
7. Apply Transfer Learning with MobileNetV2
8. Evaluate the final model

---

## Models

### Baseline CNN

The baseline model consists of:

- 3 Convolutional layers
- ReLU activation
- MaxPooling
- Dense output layer with Softmax

The model was trained from scratch.

---

### Improved CNN

To reduce overfitting, the following techniques were added:

- Dropout
- Early Stopping

---

### Transfer Learning

The final model uses **MobileNetV2** pre-trained on ImageNet.

The convolutional base was frozen and only the classification head was trained for the Animals-10 dataset.

---

## Results

| Model | Validation Accuracy |
|-------|--------------------:|
| Baseline CNN | **68.83%** |
| MobileNetV2 | **93.52%** |

Final evaluation of MobileNetV2:

- Accuracy: **94%**
- Precision: **93%**
- Recall: **92%**
- F1-score: **93%**

---

## Conclusion

The baseline CNN successfully learned the dataset but showed signs of overfitting.

Transfer Learning with MobileNetV2 significantly improved the validation accuracy while reducing overfitting. Reusing features learned from ImageNet resulted in much better generalization compared to training a CNN from scratch.

---

## Technologies

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab

---

## Repository Structure

```
README.md
Ironhack_CNN_Animals_10_FINAL.ipynb
```

---

## Author

**Alexander Socha**

Ironhack AI Engineering Bootcamp June '26 led by Luis Junco 
