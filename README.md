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
   - The following are pictures of the top 5 frames selected from the validation dataset, along with interpretability plots (1. Gradient Saturation 2. Integral Gradient):

     
      1. Image3823.jpg
     ![Frame 1](https://drive.google.com/uc?export=view&id=1dSdpZeeZqle0b2Xppnpnbvf086SR34AA)

      2. normal_15.jpg
     ![Frame 2](https://drive.google.com/uc?export=view&id=124p-9B8LNt1D6liLL42I280Tb1gMUPyS)

      3. 23image60.jpg
     ![Frame 3](https://drive.google.com/uc?export=view&id=1wQyKXc7FqrKPVICRTh8D4CQV8bHDUBkI)

      4. pco_5.jpg
     ![Frame 4](https://drive.google.com/uc?export=view&id=1bcHIFeBYOsMxVq325pwzre0OYX11H3AA)

      5. 1image40.jpg
     ![Frame 5](https://drive.google.com/uc?export=view&id=1OeYdCvD6cgZtVQ6eTs1IXRk5TnQo00oU)

## Results on Testing Dataset

### Classification and Interpretability Plots
   - The following are pictures of the top 5 frames selected from the testing dataset, along with interpretability plots (1. Gradient Saturation 2. Integral Gradient):
      1. image10002.jpg
     ![Frame 1](https://drive.google.com/uc?export=view&id=1glX9OKb3LaHkCv1JeZacEQlDmbqpz49e)

      2. image10087.jpg
     ![Frame 2](https://drive.google.com/uc?export=view&id=1idwZ6KKJp9xfDSU9aNomCp5GD6xTBzfl)

      3. image10057.jpg
     ![Frame 3](https://drive.google.com/uc?export=view&id=1vMp7sMpIbOfRTMtZztKwioRR03Dl-8oV)

      4. image10121.jpg
     ![Frame 4](https://drive.google.com/uc?export=view&id=1JlMDFoCNeitwQHOEe3XSQIP1HQhPvnqr)

      5. image10967.jpg
     ![Frame 5](https://drive.google.com/uc?export=view&id=1i68BKZDZiv8W8LGQp5nbTN69EDQmNQRY)

