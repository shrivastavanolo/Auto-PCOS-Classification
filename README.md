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

### Classification and Interpretability Plots
   - The following are pictures of the top 5 frames selected from the validation dataset, along with interpretability plots at 600 DPI:
      1. ![Frame 1](https://drive.google.com/file/d/1gSq75DktbBMLnLTjCZ0QgabfAvEzgOjr/view?usp=sharing)
      2. ![Frame 2](link-to-frame2-image)
      3. ![Frame 3](link-to-frame3-image)
      4. ![Frame 4](link-to-frame4-image)
      5. ![Frame 5](link-to-frame5-image)

## Results on Testing Dataset

### Classification and Interpretability Plots
   - The following are pictures of the top 5 frames selected from the testing dataset, along with interpretability plots at 600 DPI:
      1. ![Frame 1](link-to-test-frame1-image)
      2. ![Frame 2](link-to-test-frame2-image)
      3. ![Frame 3](link-to-test-frame3-image)
      4. ![Frame 4](link-to-test-frame4-image)
      5. ![Frame 5](link-to-test-frame5-image)

