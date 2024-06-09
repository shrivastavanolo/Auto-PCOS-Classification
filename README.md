# Auto-PCOS-Classification
Auto-PCOS Classification Challenge Team LearnDroids

# Ultrasound Image Classification Pipeline

## Brief Write-up and Pipeline Overview

This repository contains the code for a machine learning pipeline to classify ultrasound images into healthy and unhealthy categories using a MobileNet-based model. The pipeline includes data preprocessing, model training, and evaluation.

## Pipeline Overview

1. **Data Preprocessing:**
   - The image data is read from an Excel sheet containing class labels.
   - Images are preprocessed using the MobileNet preprocessing function, including augmentation techniques like zoom, shear, and horizontal flip.

2. **Model Architecture:**
   - The base MobileNet model is utilized, with the final layer modified for binary classification.
   - The model is compiled using the Adam optimizer, binary cross-entropy loss, and multiple evaluation metrics (Recall, Accuracy, Precision, and AUC).

3. **Training:**
   - The model is trained using the specified dataset, with checkpoints and early stopping callbacks.

## Results on Validation Dataset

### Evaluation Metrics Table
| Loss   | Recall   | Accuracy   | Precision   | AUC      |
|--------|----------|------------|-------------|----------|
| 1.5586 | 0.6641   | 0.8146     | 0.6591      | 0.8049   |

