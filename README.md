# Emoji-Detection
Emoji Detection with traditional machine learning algorithms

# Emoji Classification with SVM

This repository contains a computer vision project for COMP4423 (Semester 2, 2023/24) that tackles the challenge of classifying emojis using traditional machine learning techniques.

## Project Overview

Emojis, though simple in appearance, are notoriously difficult to classify due to their high visual similarity. This project covers:
- **Data Collection & Preprocessing:** An extended, manually labeled dataset with 24 classes.
- **Feature Extraction:** Application of Sobel, Laplacian, Circular LBP, and HOG filters to extract meaningful features.
- **Image Stacking:** Combining filtered outputs to simulate a CNN-like flattening process.
- **Model Training:** Using a Support Vector Classifier (SVC) optimized with grid search and cross-validation.
- **Testing:** Achieved 60.42% accuracy on emojis, highlighting challenges when applied to human facial expressions.

## Dataset

- **Composition:** 149 training images and 48 testing images across 24 classes.
- **Challenges:** Overlapping features between classes and limited data per class, resulting in a low baseline chance of random correct classification.

![TSNE](https://github.com/user-attachments/assets/8dd34cdb-a75a-4222-9835-c641d72b8bca)


## Methods

- **Preprocessing:** Converting Unicode emojis to grayscale images.
- **Feature Extraction Techniques:**
  - *Sobel Filter:* For edge detection.
  - *Laplacian Filter:* To highlight sharp features.
  - *Circular LBP:* For capturing local texture details.
  - *HOG:* For local shape patterns.
- **Model:** A Support Vector Classifier was chosen due to its strength in handling high-dimensional, non-linear data.
- **Training & Optimization:** Employed grid search with cross-validation to fine-tune hyperparameters.

## Results & Discussion

- **Emoji Classification:** Achieved an accuracy of 60.42%.
- **Human Face Emotions:** The model scored 0% accuracy, underlining the domain-specific challenges between emojis and human expressions.
- **Future Work:** Suggests expanding the dataset with colored images and refining feature extraction techniques to reduce class overlap.
