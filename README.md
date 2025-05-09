# Image-Classification
Repository for Image Classification Projects 

## Fashion Image Classification

This repository contains a deep learning project focused on classifying fashion images into one of three categories: **Casual**, **Formal**, and **Smart Casual**. The project explores both a baseline CNN model and an enhanced version incorporating data augmentation and dropout regularization.

### Project Overview

In the notebook, a pipeline was built to:

- Load and preprocess a fashion dataset (`styles.csv` + image folder)
- Train a baseline CNN model using unaugmented image data
- Develop an enhanced CNN model using techniques such as:
  - Data augmentation
  - Batch normalization
  - Dropout layers
- Evaluate and compare both models based on accuracy and loss

The models were trained and tested using TensorFlow and Keras with clear separation between training, validation, and test sets.

### Dataset

The dataset consists of:

- `styles.csv`: Metadata and label information for each image
- `images/`: A folder of fashion item images

Only three target classes were used: **Casual**, **Formal**, and **Smart Casual**. These classes were filtered and relabeled before model training.

### Results Summary

| Model           | Validation Accuracy | Test Accuracy |
|----------------|---------------------|----------------|
| Baseline CNN   | ~85%                | ~84%           |
| Enhanced CNN   | ~96%                | ~96%           |

The enhanced model significantly outperforms the baseline, demonstrating the impact of regularization and data augmentation techniques.

### How to Run the Project

1. Clone the repository.
2. Place `styles.csv` and the `images/` folder in the root directory of the project.
3. Install the dependencies using the provided requirements file:
   ```bash
   pip install -r requirements.txt
4. Open and run the notebook cell by cell in your Jupyter environment.




